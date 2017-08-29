# <a name="list-groupsettingtemplates"></a><span data-ttu-id="92426-101">Lista groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="92426-101">List groupSettingTemplates</span></span>

<span data-ttu-id="92426-p101">Os Modelos de configuração de grupo representam um conjunto de modelos pelo qual as configurações de grupo podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos groupSettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="92426-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="92426-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="92426-104">Permissions</span></span>

<span data-ttu-id="92426-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="92426-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="92426-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92426-107">Permission type</span></span>      | <span data-ttu-id="92426-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92426-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92426-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92426-109">Delegated (work or school account)</span></span> | <span data-ttu-id="92426-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92426-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="92426-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92426-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92426-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92426-112">Not supported.</span></span>    |
|<span data-ttu-id="92426-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92426-113">Application</span></span> | <span data-ttu-id="92426-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92426-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92426-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92426-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92426-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92426-116">Optional query parameters</span></span>
<span data-ttu-id="92426-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92426-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="92426-118">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="92426-118">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92426-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92426-119">Request headers</span></span>
| <span data-ttu-id="92426-120">Nome</span><span class="sxs-lookup"><span data-stu-id="92426-120">Name</span></span> | <span data-ttu-id="92426-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="92426-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="92426-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92426-122">Authorization</span></span>  | <span data-ttu-id="92426-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92426-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92426-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92426-125">Request body</span></span>
<span data-ttu-id="92426-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92426-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92426-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="92426-127">Response</span></span>

<span data-ttu-id="92426-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92426-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92426-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92426-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92426-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92426-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="92426-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="92426-131">Response</span></span>

<span data-ttu-id="92426-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92426-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
                        }
                }
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->