## Add private name to `__all__`

You can add the private name to `__all__` When you write 'unexport: public' as a
comment.

````python
__all__ = ["name", "_protected_name", "__private_name", "_protected_function", "__private_function", "_ProtectedClass", "__PrivateClass"]

name = ... # unexport: public
_protected_name = ...  # unexport: public
__private_name = ...  # unexport: public

def _protected_function(): ...  # unexport: public
def __private_function(): ...  # unexport: public

class _ProtectedClass: ...  # unexport: public
class __PrivateClass: ...  # unexport: public

## Remove public name from `__all__`

You can remove the public name from `__all__` When you write 'unexport: not-public' as a
comment.

```python
PUBLIC_NAME = ...  # unexport: not-public

def public_function(): ...  # unexport: not-public

class PublicClass:...  # unexport: not-public

````
