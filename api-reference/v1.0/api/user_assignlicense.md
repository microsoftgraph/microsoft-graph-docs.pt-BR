# <a name="assignlicense"></a><span data-ttu-id="27417-101">assignLicense</span><span class="sxs-lookup"><span data-stu-id="27417-101">assignLicense</span></span>
<span data-ttu-id="27417-p101">Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="27417-p101">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27417-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27417-104">Prerequisites</span></span>
<span data-ttu-id="27417-105">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.ReadWrite.All; Directory.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="27417-105">One of the following **scopes** is required to execute this API: *User.ReadWrite.All; Directory.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="27417-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27417-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="27417-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27417-107">Request headers</span></span>
| <span data-ttu-id="27417-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27417-108">Header</span></span>       | <span data-ttu-id="27417-109">Valor</span><span class="sxs-lookup"><span data-stu-id="27417-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27417-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="27417-110">Authorization</span></span>  | <span data-ttu-id="27417-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27417-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27417-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27417-113">Content-Type</span></span>  | <span data-ttu-id="27417-114">application/json</span><span class="sxs-lookup"><span data-stu-id="27417-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27417-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27417-115">Request body</span></span>
<span data-ttu-id="27417-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27417-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27417-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27417-117">Parameter</span></span>    | <span data-ttu-id="27417-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="27417-118">Type</span></span>   |<span data-ttu-id="27417-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="27417-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27417-120">addLicenses</span><span class="sxs-lookup"><span data-stu-id="27417-120">addLicenses</span></span>|<span data-ttu-id="27417-121">AssignedLicense</span><span class="sxs-lookup"><span data-stu-id="27417-121">AssignedLicense</span></span>|<span data-ttu-id="27417-p103">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar. Você pode desabilitar os planos associados a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="27417-p103">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="27417-124">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="27417-124">removeLicenses</span></span>|<span data-ttu-id="27417-125">Guid</span><span class="sxs-lookup"><span data-stu-id="27417-125">Guid</span></span>|<span data-ttu-id="27417-126">Uma coleção de GUIDs que identifica as licenças a remover.</span><span class="sxs-lookup"><span data-stu-id="27417-126">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="27417-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="27417-127">Response</span></span>

<span data-ttu-id="27417-128">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27417-128">If successful, this method returns `200, OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27417-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27417-129">Example</span></span>
<span data-ttu-id="27417-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="27417-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="27417-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27417-131">Request</span></span>
<span data-ttu-id="27417-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27417-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="27417-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27417-133">Response</span></span>
<span data-ttu-id="27417-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27417-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
