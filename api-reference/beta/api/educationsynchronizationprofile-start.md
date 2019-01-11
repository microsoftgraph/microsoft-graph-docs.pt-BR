---
title: Iniciar sincronização após o carregamento de arquivos para um educationSynchronizationProfile
description: Verifique se os arquivos carregados para um perfil de sincronização de dados escola específico no inquilino. Se a verificação for bem-sucedida, a sincronização será iniciado no perfil. Caso contrário, a resposta conterá erros e avisos. Se a resposta contiver erros, a sincronização não será iniciado. Se a resposta conterá apenas avisos, sincronização será iniciado.
localization_priority: Normal
ms.openlocfilehash: 465ab6a807fc6af10067d048459c440c7c567361
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866735"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="e892e-107">Iniciar sincronização após o carregamento de arquivos para um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e892e-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

> <span data-ttu-id="e892e-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e892e-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e892e-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e892e-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e892e-110">Verifique se os arquivos carregados para um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="e892e-110">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="e892e-111">Se a verificação for bem-sucedida, a sincronização será iniciado no perfil.</span><span class="sxs-lookup"><span data-stu-id="e892e-111">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="e892e-112">Caso contrário, a resposta conterá erros e avisos.</span><span class="sxs-lookup"><span data-stu-id="e892e-112">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="e892e-113">Se a resposta contiver erros, a sincronização não será iniciado.</span><span class="sxs-lookup"><span data-stu-id="e892e-113">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="e892e-114">Se a resposta conterá apenas avisos, sincronização será iniciado.</span><span class="sxs-lookup"><span data-stu-id="e892e-114">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="e892e-115">**Observação:** Use este método somente quando o provedor de dados é do tipo [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e892e-115">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="e892e-116">Além disso, a propriedade de estado do perfil precisa ser provisionado para que ela pode ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="e892e-116">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="e892e-117">Sondar o objeto de perfil para verificar sua propriedade state.</span><span class="sxs-lookup"><span data-stu-id="e892e-117">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e892e-118">Permissions</span><span class="sxs-lookup"><span data-stu-id="e892e-118">Permissions</span></span>
<span data-ttu-id="e892e-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e892e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e892e-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e892e-121">Permission type</span></span> | <span data-ttu-id="e892e-122">Permissions</span><span class="sxs-lookup"><span data-stu-id="e892e-122">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e892e-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e892e-123">Delegated (work or school account)</span></span> | <span data-ttu-id="e892e-124">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e892e-124">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e892e-125">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e892e-125">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e892e-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e892e-126">Not supported.</span></span>|
|<span data-ttu-id="e892e-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e892e-127">Application</span></span>|<span data-ttu-id="e892e-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e892e-128">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e892e-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e892e-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="e892e-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e892e-130">Request headers</span></span>
| <span data-ttu-id="e892e-131">Nome</span><span class="sxs-lookup"><span data-stu-id="e892e-131">Name</span></span>       | <span data-ttu-id="e892e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e892e-132">Type</span></span> | <span data-ttu-id="e892e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e892e-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e892e-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="e892e-134">Authorization</span></span>  | <span data-ttu-id="e892e-135">string</span><span class="sxs-lookup"><span data-stu-id="e892e-135">string</span></span>  | <span data-ttu-id="e892e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e892e-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e892e-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e892e-138">Request body</span></span>
<span data-ttu-id="e892e-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e892e-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e892e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e892e-140">Response</span></span>
<span data-ttu-id="e892e-141">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e892e-141">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="e892e-142">Se não obtiver êxito, será retornado um `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="e892e-142">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="e892e-143">A resposta conterá uma coleção de objetos de [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) como parte do corpo da resposta se existem erros ou avisos encontrados.</span><span class="sxs-lookup"><span data-stu-id="e892e-143">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="e892e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e892e-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e892e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e892e-145">Request</span></span>
<span data-ttu-id="e892e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e892e-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="e892e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e892e-147">Response</span></span>
<span data-ttu-id="e892e-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e892e-148">Here is an example of the response.</span></span> 

><span data-ttu-id="e892e-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e892e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
