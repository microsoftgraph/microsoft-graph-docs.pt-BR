# <a name="update-educationclass-properties"></a><span data-ttu-id="b5536-101">Atualizar propriedades educationclass</span><span class="sxs-lookup"><span data-stu-id="b5536-101">Update educationclass properties</span></span>

<span data-ttu-id="b5536-102">Atualize as propriedades de uma aula.</span><span class="sxs-lookup"><span data-stu-id="b5536-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5536-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5536-103">Permissions</span></span>
<span data-ttu-id="b5536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5536-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5536-106">Permission type</span></span>      | <span data-ttu-id="b5536-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5536-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5536-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5536-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="b5536-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5536-109">Not supported.</span></span>  |
|<span data-ttu-id="b5536-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5536-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5536-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5536-111">Not supported.</span></span>   |
|<span data-ttu-id="b5536-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5536-112">Application</span></span> | <span data-ttu-id="b5536-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5536-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b5536-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5536-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b5536-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5536-115">Request headers</span></span>
| <span data-ttu-id="b5536-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5536-116">Header</span></span>       | <span data-ttu-id="b5536-117">Valor</span><span class="sxs-lookup"><span data-stu-id="b5536-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5536-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5536-118">Authorization</span></span>  | <span data-ttu-id="b5536-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5536-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b5536-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5536-121">Content-Type</span></span>  | <span data-ttu-id="b5536-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b5536-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5536-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5536-123">Request body</span></span>
<span data-ttu-id="b5536-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b5536-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b5536-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b5536-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b5536-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b5536-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b5536-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5536-127">Property</span></span>     | <span data-ttu-id="b5536-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5536-128">Type</span></span>   |<span data-ttu-id="b5536-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5536-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5536-130">description</span><span class="sxs-lookup"><span data-stu-id="b5536-130">description</span></span>|<span data-ttu-id="b5536-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5536-131">String</span></span>| <span data-ttu-id="b5536-132">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="b5536-132">Description of the template.</span></span>|
|<span data-ttu-id="b5536-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b5536-133">displayName</span></span>|<span data-ttu-id="b5536-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5536-134">String</span></span>| <span data-ttu-id="b5536-135">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="b5536-135">Name of the class.</span></span>|
|<span data-ttu-id="b5536-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b5536-136">mailNickname</span></span>|<span data-ttu-id="b5536-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5536-137">String</span></span>| <span data-ttu-id="b5536-138">Alias de email para envio de email a todos os usuários, se esse recurso estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="b5536-138">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="b5536-139">|classCode|Cadeia de caracteres| Código de aula usado pela escola.| |externalId|Cadeia de caracteres| ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="b5536-139">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="b5536-140">| |externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.| |externalSource|cadeia de caracteres| Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="b5536-140">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="b5536-141">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.|</span><span class="sxs-lookup"><span data-stu-id="b5536-141">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>

## <a name="response"></a><span data-ttu-id="b5536-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5536-142">Response</span></span>
<span data-ttu-id="b5536-143">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5536-143">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5536-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5536-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5536-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5536-145">Request</span></span>
<span data-ttu-id="b5536-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5536-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="b5536-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5536-147">Response</span></span>
<span data-ttu-id="b5536-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5536-148">The following is an example of the response.</span></span> 

><span data-ttu-id="b5536-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5536-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->