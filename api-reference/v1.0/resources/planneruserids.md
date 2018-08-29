# <a name="planneruserids-resource-type"></a><span data-ttu-id="a5a31-101">Tipo de recurso plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="a5a31-101">plannerUserIds resource type</span></span>

<span data-ttu-id="a5a31-p101">O recurso **plannerUserIds** representa a lista de ids de usuários com a qual um [plano](plannerplan.md) é compartilhado. Este é um Tipo Aberto. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.</span><span class="sxs-lookup"><span data-stu-id="a5a31-p101">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with. This is an Open Type. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="a5a31-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5a31-106">Properties</span></span>
<span data-ttu-id="a5a31-p102">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer identificações de usuário como propriedades e seus valores devem ser o booliano `true`. Quando as identificações de usuário já não forem compartilhadas, as propriedades serão automaticamente removidas ao configurar os valores com o booliano `false`.</span><span class="sxs-lookup"><span data-stu-id="a5a31-p102">Properties of an Open Type can be defined by the client. In this case, the client should provide user ids as properties with their values being the `true` boolean. When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a5a31-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5a31-110">JSON representation</span></span>

<span data-ttu-id="a5a31-111">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a5a31-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="a5a31-112">// Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5a31-112">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->