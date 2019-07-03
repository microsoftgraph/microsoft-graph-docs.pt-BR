---
title: Iniciar sincronização após carregar arquivos em um educationSynchronizationProfile
description: Verifique se os arquivos foram carregados em um perfil de sincronização de dados escolar específico no locatário. Se a verificação for bem-sucedida, a sincronização será iniciada no perfil. Caso contrário, a resposta conterá erros e avisos. Se a resposta contiver erros, a sincronização não será iniciada. Se a resposta contiver apenas avisos, a sincronização será iniciada.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2c571ca614c8bb97babe93537e99606ce8799b0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441272"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="7afd1-107">Iniciar sincronização após carregar arquivos em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="7afd1-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7afd1-108">Verifique se os arquivos foram carregados em um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="7afd1-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="7afd1-109">Se a verificação for bem-sucedida, a sincronização será iniciada no perfil.</span><span class="sxs-lookup"><span data-stu-id="7afd1-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="7afd1-110">Caso contrário, a resposta conterá erros e avisos.</span><span class="sxs-lookup"><span data-stu-id="7afd1-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="7afd1-111">Se a resposta contiver erros, a sincronização não será iniciada.</span><span class="sxs-lookup"><span data-stu-id="7afd1-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="7afd1-112">Se a resposta contiver apenas avisos, a sincronização será iniciada.</span><span class="sxs-lookup"><span data-stu-id="7afd1-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="7afd1-113">**Observação:** Use este método somente quando o provedor de dados for do tipo [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="7afd1-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="7afd1-114">Além disso, a propriedade State do perfil precisa ser provisionada para que possa ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="7afd1-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="7afd1-115">Sondar o objeto de perfil para verificar sua propriedade State.</span><span class="sxs-lookup"><span data-stu-id="7afd1-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7afd1-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="7afd1-116">Permissions</span></span>
<span data-ttu-id="7afd1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7afd1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7afd1-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7afd1-119">Permission type</span></span> | <span data-ttu-id="7afd1-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="7afd1-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7afd1-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7afd1-121">Delegated (work or school account)</span></span> | <span data-ttu-id="7afd1-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afd1-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7afd1-123">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="7afd1-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7afd1-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7afd1-124">Not supported.</span></span>|
|<span data-ttu-id="7afd1-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7afd1-125">Application</span></span>|<span data-ttu-id="7afd1-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7afd1-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7afd1-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7afd1-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="7afd1-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7afd1-128">Request headers</span></span>
| <span data-ttu-id="7afd1-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7afd1-129">Name</span></span>       | <span data-ttu-id="7afd1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7afd1-130">Type</span></span> | <span data-ttu-id="7afd1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7afd1-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7afd1-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="7afd1-132">Authorization</span></span>  | <span data-ttu-id="7afd1-133">string</span><span class="sxs-lookup"><span data-stu-id="7afd1-133">string</span></span>  | <span data-ttu-id="7afd1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7afd1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7afd1-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7afd1-136">Request body</span></span>
<span data-ttu-id="7afd1-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7afd1-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7afd1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7afd1-138">Response</span></span>
<span data-ttu-id="7afd1-139">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="7afd1-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="7afd1-140">Se não tiver êxito, retornará um `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="7afd1-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="7afd1-141">A resposta contém uma coleção de objetos [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) como parte do corpo da resposta se forem encontrados erros ou avisos.</span><span class="sxs-lookup"><span data-stu-id="7afd1-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="7afd1-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7afd1-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7afd1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7afd1-143">Request</span></span>
<span data-ttu-id="7afd1-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7afd1-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7afd1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7afd1-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7afd1-146">C#</span><span class="sxs-lookup"><span data-stu-id="7afd1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7afd1-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="7afd1-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7afd1-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7afd1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7afd1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7afd1-149">Response</span></span>
<span data-ttu-id="7afd1-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7afd1-150">Here is an example of the response.</span></span> 

><span data-ttu-id="7afd1-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7afd1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
