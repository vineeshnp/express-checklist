# Express Check List #
=============

More the people using something in cloud, the chances of getting hacked increases. Since express is being used in a huge magnitude
here is a set of check list that we should follow before deploying express code to server.

- [ ] Make sure version of node is LTS on the live-server.
- [ ] Use https or TLS. [Lets Encrypt](https://letsencrypt.org/) Could be used to enable this
- [ ] Disable non standard headers ```js app.disable('x-powered-by') ` `` 
- [ ] Use [helmet](https://www.npmjs.com/package/helmet).
- [ ] Run [nsp](https://www.npmjs.com/package/nsp) to check identify known vulnerabilities. 
- [ ] Run [sync](https://www.npmjs.com/package/snyk) for further vulnerabilities check.
- [ ] Take a look at reported [vulnerabilities](https://nodesecurity.io/advisories)
- [ ] Use [express-limiter](https://www.npmjs.com/package/express-limiter) on the auth api's
- [ ] Use [csurf](https://www.npmjs.com/package/csurf) to block CSRF.
- [ ] Test with [sqlmap](http://sqlmap.org/) before going live.
- [ ] Use [safe-regex](https://www.npmjs.com/package/safe-regex) if regular expressions are used in the code to prevent from [ReDos](https://www.owasp.org/index.php/Regular_expression_Denial_of_Service_-_ReDoS)
- [ ] Run [nmap](https://nmap.org/) at the time of deployment.
- [ ] Run [sslyze](https://github.com/nabla-c0d3/sslyze) To figure out vulnerabilities on ssl.


# Gratitude #
=============
Thanks to the blog from [express](https://expressjs.com/en/advanced/best-practice-security.html) team.
