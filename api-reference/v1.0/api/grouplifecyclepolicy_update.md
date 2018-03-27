# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="7e8ca-101">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7e8ca-101">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="7e8ca-102">Atualiza as propriedades de um objeto do [tipo de recurso groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7e8ca-102">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e8ca-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e8ca-103">Permissions</span></span>

<span data-ttu-id="7e8ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e8ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 
|<span data-ttu-id="7e8ca-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e8ca-106">Permission type</span></span>      | <span data-ttu-id="7e8ca-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e8ca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e8ca-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e8ca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7e8ca-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e8ca-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e8ca-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e8ca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e8ca-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-111">Not supported.</span></span>    |
|<span data-ttu-id="7e8ca-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e8ca-112">Application</span></span> | <span data-ttu-id="7e8ca-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e8ca-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e8ca-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e8ca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7e8ca-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7e8ca-115">Optional request headers</span></span>
| <span data-ttu-id="7e8ca-116">Nome</span><span class="sxs-lookup"><span data-stu-id="7e8ca-116">Name</span></span> | <span data-ttu-id="7e8ca-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e8ca-117">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="7e8ca-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e8ca-118">Authorization</span></span> | <span data-ttu-id="7e8ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e8ca-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e8ca-121">Content-Type</span></span>  | <span data-ttu-id="7e8ca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7e8ca-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e8ca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e8ca-123">Request body</span></span>

<span data-ttu-id="7e8ca-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7e8ca-125">As propriedades existentes que não estão incluídas no corpo da solicitação mantêm os valores anteriores ou recalcula-os com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7e8ca-126">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e8ca-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e8ca-127">Property</span></span> | <span data-ttu-id="7e8ca-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e8ca-128">Type</span></span> | <span data-ttu-id="7e8ca-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e8ca-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7e8ca-130">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="7e8ca-130">alternateNotificationEmails</span></span>|<span data-ttu-id="7e8ca-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e8ca-131">String</span></span>| <span data-ttu-id="7e8ca-132">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-132">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="7e8ca-133">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-133">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="7e8ca-134">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="7e8ca-134">groupLifetimeInDays</span></span>|<span data-ttu-id="7e8ca-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7e8ca-135">Int32</span></span>| <span data-ttu-id="7e8ca-136">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-136">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="7e8ca-137">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-137">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="7e8ca-138">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="7e8ca-138">managedGroupTypes</span></span>|<span data-ttu-id="7e8ca-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e8ca-139">String</span></span>| <span data-ttu-id="7e8ca-140">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-140">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="7e8ca-141">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-141">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="7e8ca-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e8ca-142">Response</span></span>

<span data-ttu-id="7e8ca-143">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-143">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e8ca-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e8ca-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e8ca-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e8ca-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="7e8ca-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e8ca-146">Response</span></span>
<span data-ttu-id="7e8ca-147">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7e8ca-147">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->