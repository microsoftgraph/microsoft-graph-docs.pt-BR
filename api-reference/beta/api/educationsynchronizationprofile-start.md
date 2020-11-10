---
title: Iniciar sincronização após carregar arquivos em um educationSynchronizationProfile
description: Verifique se os arquivos foram carregados em um perfil de sincronização de dados escolar específico no locatário. Se a verificação for bem-sucedida, a sincronização será iniciada no perfil. Caso contrário, a resposta conterá erros e avisos. Se a resposta contiver erros, a sincronização não será iniciada. Se a resposta contiver apenas avisos, a sincronização será iniciada.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7953171f90c5b9297bca1122cfe21b3ad854287a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965794"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="b11cd-107">Iniciar sincronização após carregar arquivos em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="b11cd-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

<span data-ttu-id="b11cd-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b11cd-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b11cd-109">Verifique se os arquivos foram carregados em um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="b11cd-109">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="b11cd-110">Se a verificação for bem-sucedida, a sincronização será iniciada no perfil.</span><span class="sxs-lookup"><span data-stu-id="b11cd-110">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="b11cd-111">Caso contrário, a resposta conterá erros e avisos.</span><span class="sxs-lookup"><span data-stu-id="b11cd-111">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="b11cd-112">Se a resposta contiver erros, a sincronização não será iniciada.</span><span class="sxs-lookup"><span data-stu-id="b11cd-112">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="b11cd-113">Se a resposta contiver apenas avisos, a sincronização será iniciada.</span><span class="sxs-lookup"><span data-stu-id="b11cd-113">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="b11cd-114">**Observação:** Use este método somente quando o provedor de dados for do tipo [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b11cd-114">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="b11cd-115">Além disso, a propriedade State do perfil precisa ser provisionada para que possa ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="b11cd-115">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="b11cd-116">Sondar o objeto de perfil para verificar sua propriedade State.</span><span class="sxs-lookup"><span data-stu-id="b11cd-116">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b11cd-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="b11cd-117">Permissions</span></span>
<span data-ttu-id="b11cd-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b11cd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b11cd-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b11cd-120">Permission type</span></span> | <span data-ttu-id="b11cd-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="b11cd-121">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b11cd-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b11cd-122">Delegated (work or school account)</span></span> | <span data-ttu-id="b11cd-123">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b11cd-123">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="b11cd-124">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b11cd-124">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b11cd-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b11cd-125">Not supported.</span></span>|
|<span data-ttu-id="b11cd-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b11cd-126">Application</span></span>|<span data-ttu-id="b11cd-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b11cd-127">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b11cd-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b11cd-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="b11cd-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b11cd-129">Request headers</span></span>
| <span data-ttu-id="b11cd-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b11cd-130">Name</span></span>       | <span data-ttu-id="b11cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b11cd-131">Type</span></span> | <span data-ttu-id="b11cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b11cd-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b11cd-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="b11cd-133">Authorization</span></span>  | <span data-ttu-id="b11cd-134">string</span><span class="sxs-lookup"><span data-stu-id="b11cd-134">string</span></span>  | <span data-ttu-id="b11cd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b11cd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b11cd-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b11cd-137">Request body</span></span>
<span data-ttu-id="b11cd-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b11cd-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b11cd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b11cd-139">Response</span></span>
<span data-ttu-id="b11cd-140">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b11cd-140">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="b11cd-141">Se não tiver êxito, retornará um `400 Bad Request` .</span><span class="sxs-lookup"><span data-stu-id="b11cd-141">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="b11cd-142">A resposta contém uma coleção de objetos [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) como parte do corpo da resposta se forem encontrados erros ou avisos.</span><span class="sxs-lookup"><span data-stu-id="b11cd-142">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="b11cd-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b11cd-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b11cd-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b11cd-144">Request</span></span>
<span data-ttu-id="b11cd-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b11cd-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b11cd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b11cd-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="c"></a>[<span data-ttu-id="b11cd-147">C#</span><span class="sxs-lookup"><span data-stu-id="b11cd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b11cd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b11cd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b11cd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b11cd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b11cd-150">Java</span><span class="sxs-lookup"><span data-stu-id="b11cd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b11cd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b11cd-151">Response</span></span>
<span data-ttu-id="b11cd-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b11cd-152">Here is an example of the response.</span></span> 

><span data-ttu-id="b11cd-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b11cd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


