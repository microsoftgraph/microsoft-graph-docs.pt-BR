# <a name="passwordprofile-resource-type"></a><span data-ttu-id="1a821-101">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="1a821-101">passwordProfile resource type</span></span>

<span data-ttu-id="1a821-p101">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="1a821-p101">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="1a821-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a821-104">Properties</span></span>
| <span data-ttu-id="1a821-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a821-105">Property</span></span>     | <span data-ttu-id="1a821-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a821-106">Type</span></span>   |<span data-ttu-id="1a821-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a821-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a821-108">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="1a821-108">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="1a821-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a821-109">Boolean</span></span>| <span data-ttu-id="1a821-110">**true** se o usuário precisa alterar sua senha no próximo login; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="1a821-110">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="1a821-111">password</span><span class="sxs-lookup"><span data-stu-id="1a821-111">password</span></span>|<span data-ttu-id="1a821-112">String</span><span class="sxs-lookup"><span data-stu-id="1a821-112">String</span></span>|<span data-ttu-id="1a821-p102">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="1a821-p102">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a821-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a821-118">JSON representation</span></span>

<span data-ttu-id="1a821-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1a821-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->