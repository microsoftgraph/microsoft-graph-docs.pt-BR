---
title: Iniciar a sincronização depois de carregar arquivos em um educationSynchronizationProfile
description: Verifique os arquivos carregados em um perfil específico de sincronização de dados escolares no locatário. Se a verificação for bem-sucedida, a sincronização começará no perfil. Caso contrário, a resposta conterá erros e avisos. Se a resposta contiver erros, a sincronização não será iniciar. Se a resposta contiver apenas avisos, a sincronização será iniciar.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 04f8f9e96422c262ea816a5f24796d4059b0809c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574141"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="e35e0-107">Iniciar a sincronização depois de carregar arquivos em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e35e0-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

<span data-ttu-id="e35e0-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e35e0-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35e0-109">Verifique os arquivos carregados em um perfil específico de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolares no locatário.</span><span class="sxs-lookup"><span data-stu-id="e35e0-109">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="e35e0-110">Se a verificação for bem-sucedida, a sincronização começará no perfil.</span><span class="sxs-lookup"><span data-stu-id="e35e0-110">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="e35e0-111">Caso contrário, a resposta conterá erros e avisos.</span><span class="sxs-lookup"><span data-stu-id="e35e0-111">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="e35e0-112">Se a resposta contiver erros, a sincronização não será iniciar.</span><span class="sxs-lookup"><span data-stu-id="e35e0-112">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="e35e0-113">Se a resposta contiver apenas avisos, a sincronização será iniciar.</span><span class="sxs-lookup"><span data-stu-id="e35e0-113">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="e35e0-114">**Observação:** Use esse método somente quando o provedor de dados for do tipo [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e35e0-114">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="e35e0-115">Além disso, a propriedade de estado do perfil precisa ser provisionada antes que ela possa ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="e35e0-115">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="e35e0-116">Sondar o objeto profile para verificar sua propriedade de estado.</span><span class="sxs-lookup"><span data-stu-id="e35e0-116">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e35e0-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="e35e0-117">Permissions</span></span>
<span data-ttu-id="e35e0-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e35e0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e35e0-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e35e0-120">Permission type</span></span> | <span data-ttu-id="e35e0-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="e35e0-121">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e35e0-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e35e0-122">Delegated (work or school account)</span></span> | <span data-ttu-id="e35e0-123">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e35e0-123">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e35e0-124">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e35e0-124">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e35e0-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e35e0-125">Not supported.</span></span>|
|<span data-ttu-id="e35e0-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e35e0-126">Application</span></span>|<span data-ttu-id="e35e0-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e35e0-127">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e35e0-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e35e0-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="e35e0-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e35e0-129">Request headers</span></span>
| <span data-ttu-id="e35e0-130">Nome</span><span class="sxs-lookup"><span data-stu-id="e35e0-130">Name</span></span>       | <span data-ttu-id="e35e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e35e0-131">Type</span></span> | <span data-ttu-id="e35e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35e0-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e35e0-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="e35e0-133">Authorization</span></span>  | <span data-ttu-id="e35e0-134">string</span><span class="sxs-lookup"><span data-stu-id="e35e0-134">string</span></span>  | <span data-ttu-id="e35e0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e35e0-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e35e0-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e35e0-137">Request body</span></span>
<span data-ttu-id="e35e0-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e35e0-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e35e0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35e0-139">Response</span></span>
<span data-ttu-id="e35e0-140">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e35e0-140">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="e35e0-141">Se não tiver êxito, retornará `400 Bad Request` um .</span><span class="sxs-lookup"><span data-stu-id="e35e0-141">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="e35e0-142">A resposta contém uma coleção de objetos [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) como parte do corpo da resposta se quaisquer erros ou avisos foram encontrados.</span><span class="sxs-lookup"><span data-stu-id="e35e0-142">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="e35e0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e35e0-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e35e0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e35e0-144">Request</span></span>
<span data-ttu-id="e35e0-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e35e0-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e35e0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e35e0-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="c"></a>[<span data-ttu-id="e35e0-147">C#</span><span class="sxs-lookup"><span data-stu-id="e35e0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e35e0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e35e0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e35e0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e35e0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e35e0-150">Java</span><span class="sxs-lookup"><span data-stu-id="e35e0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e35e0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35e0-151">Response</span></span>
<span data-ttu-id="e35e0-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e35e0-152">Here is an example of the response.</span></span> 

><span data-ttu-id="e35e0-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e35e0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


