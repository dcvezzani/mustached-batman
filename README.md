This modifies the STS example service (provided with the distribution of apache-cxf-2.7.4) into an example of message-level encryption only.

Please see README.txt (in this repository) for details on installing and running the example.  Everything is the same except there is no STS in the mix, so <code>mvn -Psts</code> should not be run.

The distribution of the Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files includes instructions on how to install.  I will only confirm that the Apache CXF instructions are correct, that the JCE libraries must replace the existing ones.  If you have multiple versions of Java JDK/JRE installed, be sure you isolate which one you are using in your environment so you update the correct files.

To run the encrypted examples, use the <code>master</code> or <code>encrypted</code> branch.

    git checkout master
    git checkout encrypted

To compare with an unencrypted example, use the <code>unencrypted</code> branch.

    git checkout unencrypted

