# Doctrine Collections

[![Join the chat at https://gitter.im/gabrielbull/collections](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/gabrielbull/collections?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Collections Abstraction library

## Changelog

### v1.2

* Add a new ``AbstractLazyCollection``

### v1.1

* Deprecated ``Comparison::IS``, because it's only there for SQL semantics.
  These are fixed in the ORM instead.
* Add ``Comparison::CONTAINS`` to perform partial string matches:

        $criteria->andWhere($criteria->expr()->contains('property', 'Foo'));
