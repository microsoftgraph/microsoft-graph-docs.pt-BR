# <a name="update-educationuser-properties"></a><span data-ttu-id="5b504-101">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="5b504-101">Update educationUser properties</span></span>

<span data-ttu-id="5b504-102">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="5b504-102">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b504-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b504-103">Permissions</span></span>
<span data-ttu-id="5b504-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5b504-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b504-106">Permission type</span></span>      | <span data-ttu-id="5b504-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b504-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b504-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b504-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="5b504-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b504-109">Not supported.</span></span>  |
|<span data-ttu-id="5b504-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b504-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5b504-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b504-111">Not supported.</span></span>  |
|<span data-ttu-id="5b504-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b504-112">Application</span></span> | <span data-ttu-id="5b504-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b504-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b504-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b504-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5b504-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b504-115">Request headers</span></span>
| <span data-ttu-id="5b504-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b504-116">Header</span></span>       | <span data-ttu-id="5b504-117">Valor</span><span class="sxs-lookup"><span data-stu-id="5b504-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b504-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b504-118">Authorization</span></span>  | <span data-ttu-id="5b504-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b504-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b504-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b504-121">Content-Type</span></span>  | <span data-ttu-id="5b504-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5b504-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b504-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b504-123">Request body</span></span>
<span data-ttu-id="5b504-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5b504-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5b504-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5b504-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b504-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5b504-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5b504-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b504-127">Property</span></span>     | <span data-ttu-id="5b504-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b504-128">Type</span></span>   |<span data-ttu-id="5b504-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b504-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b504-130">displayName</span><span class="sxs-lookup"><span data-stu-id="5b504-130">displayName</span></span>| <span data-ttu-id="5b504-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-131">String</span></span>| <span data-ttu-id="5b504-132">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="5b504-132">Display Name of User</span></span>|
|<span data-ttu-id="5b504-133">givenName</span><span class="sxs-lookup"><span data-stu-id="5b504-133">givenName</span></span>| <span data-ttu-id="5b504-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-134">String</span></span> | <span data-ttu-id="5b504-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5b504-135">First Name</span></span> |
|<span data-ttu-id="5b504-136">middleName</span><span class="sxs-lookup"><span data-stu-id="5b504-136">middleName</span></span>| <span data-ttu-id="5b504-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-137">String</span></span> | <span data-ttu-id="5b504-138">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="5b504-138">Middle Name of user</span></span>|
|<span data-ttu-id="5b504-139">surname</span><span class="sxs-lookup"><span data-stu-id="5b504-139">surname</span></span>| <span data-ttu-id="5b504-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-140">String</span></span> | <span data-ttu-id="5b504-141">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="5b504-141">Surname of user</span></span>|
|<span data-ttu-id="5b504-142">mail</span><span class="sxs-lookup"><span data-stu-id="5b504-142">mail</span></span>| <span data-ttu-id="5b504-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-143">String</span></span>| <span data-ttu-id="5b504-144">endereço de email</span><span class="sxs-lookup"><span data-stu-id="5b504-144">email address</span></span>|
|<span data-ttu-id="5b504-145">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="5b504-145">mobilePhone</span></span>| <span data-ttu-id="5b504-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-146">String</span></span> | <span data-ttu-id="5b504-147">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="5b504-147">Mobile number of user</span></span> |
|<span data-ttu-id="5b504-148">externalSource</span><span class="sxs-lookup"><span data-stu-id="5b504-148">externalSource</span></span>|<span data-ttu-id="5b504-149">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-149">string</span></span>| <span data-ttu-id="5b504-150">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="5b504-150">The possible values are:</span></span>|
|<span data-ttu-id="5b504-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="5b504-151">externalSource</span></span>|<span data-ttu-id="5b504-152">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-152">string</span></span>| <span data-ttu-id="5b504-153">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="5b504-153">Where this user was created from.</span></span>  <span data-ttu-id="5b504-154">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="5b504-154">The possible values are:</span></span>|
|<span data-ttu-id="5b504-155">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="5b504-155">mailingAddress</span></span>|[<span data-ttu-id="5b504-156">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5b504-156">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="5b504-157">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b504-157">Mail address of user.</span></span>|
|<span data-ttu-id="5b504-158">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="5b504-158">residenceAddress</span></span>|[<span data-ttu-id="5b504-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5b504-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="5b504-160">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="5b504-160">Address where user lives.</span></span>|
|<span data-ttu-id="5b504-161">primaryRole</span><span class="sxs-lookup"><span data-stu-id="5b504-161">primaryRole</span></span>|<span data-ttu-id="5b504-162">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b504-162">string</span></span>| <span data-ttu-id="5b504-163">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5b504-163">Default Role for a user.</span></span>  <span data-ttu-id="5b504-164">A função do usuário pode ser diferente em uma classe individual.</span><span class="sxs-lookup"><span data-stu-id="5b504-164">The user's role might be different in an individual class.</span></span> <span data-ttu-id="5b504-165">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="5b504-165">The possible values are:</span></span>|
|<span data-ttu-id="5b504-166">student</span><span class="sxs-lookup"><span data-stu-id="5b504-166">student</span></span>|[<span data-ttu-id="5b504-167">educationStudent</span><span class="sxs-lookup"><span data-stu-id="5b504-167">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="5b504-168">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="5b504-168">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="5b504-169">teacher</span><span class="sxs-lookup"><span data-stu-id="5b504-169">teacher</span></span>|[<span data-ttu-id="5b504-170">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="5b504-170">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="5b504-171">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="5b504-171">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="5b504-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b504-172">Response</span></span>
<span data-ttu-id="5b504-173">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b504-173">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b504-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b504-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b504-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b504-175">Request</span></span>
<span data-ttu-id="5b504-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b504-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a><span data-ttu-id="5b504-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b504-177">Response</span></span>
<span data-ttu-id="5b504-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b504-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->