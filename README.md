# Yarn Test Monorepo

Tests yarn 4.8.1.

Run `yarn`, note peerDependency errors in the install. You can change back to 4.2.2 to see this used to work.

If the answer is to use devDependencies everywhere, then add those line items by copying them from the peerDependency entry.
Run `yarn` again and notice the errors are indeed gone. But then check for node_modules, use `yarn why react`, and look in the yarn.lock to see that multiple copies of React have been installed.
