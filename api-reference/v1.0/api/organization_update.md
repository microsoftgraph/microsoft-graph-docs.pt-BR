# <a name="update-organization"></a><span data-ttu-id="81059-101">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="81059-101">Update organization</span></span>

<span data-ttu-id="81059-102">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="81059-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="81059-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="81059-103">Permissions</span></span>

<span data-ttu-id="81059-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81059-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81059-106">Permission type</span></span> | <span data-ttu-id="81059-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81059-107">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81059-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81059-108">Delegated (work or school account)</span></span> | <span data-ttu-id="81059-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81059-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81059-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81059-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81059-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81059-111">Not supported.</span></span>    |
|<span data-ttu-id="81059-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81059-112">Application</span></span> | <span data-ttu-id="81059-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81059-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81059-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81059-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="81059-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81059-115">Request headers</span></span>

| <span data-ttu-id="81059-116">Nome</span><span class="sxs-lookup"><span data-stu-id="81059-116">Name</span></span>       | <span data-ttu-id="81059-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="81059-117">Type</span></span> | <span data-ttu-id="81059-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="81059-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81059-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="81059-119">Authorization</span></span>  | <span data-ttu-id="81059-120">string</span><span class="sxs-lookup"><span data-stu-id="81059-120">string</span></span>  | <span data-ttu-id="81059-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81059-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81059-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81059-123">Request body</span></span>
<span data-ttu-id="81059-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="81059-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="81059-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="81059-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="81059-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="81059-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="81059-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81059-127">Property</span></span>     | <span data-ttu-id="81059-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="81059-128">Type</span></span>   |<span data-ttu-id="81059-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="81059-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81059-130">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="81059-130">marketingNotificationEmails</span></span>|<span data-ttu-id="81059-131">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81059-131">String collection</span></span>|                                        <span data-ttu-id="81059-132">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="81059-132">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="81059-133">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="81059-133">privacyProfile</span></span>|[<span data-ttu-id="81059-134">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="81059-134">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="81059-135">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="81059-135">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="81059-136">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="81059-136">securityComplianceNotificationMails</span></span>|<span data-ttu-id="81059-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="81059-137">String collection</span></span>||
|<span data-ttu-id="81059-138">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="81059-138">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="81059-139">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81059-139">String collection</span></span>||
|<span data-ttu-id="81059-140">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="81059-140">technicalNotificationMails</span></span>|<span data-ttu-id="81059-141">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81059-141">String collection</span></span>|                                        <span data-ttu-id="81059-142">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="81059-142">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="81059-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="81059-143">Response</span></span>

<span data-ttu-id="81059-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="81059-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="81059-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81059-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="81059-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81059-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="81059-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="81059-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
