---
title: ação uploadNewVersion
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e82db2fcbcd33e43c61a51aa011d0063a358f37a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224673"
---
# <a name="uploadnewversion-action"></a><span data-ttu-id="b6d6b-103">ação uploadNewVersion</span><span class="sxs-lookup"><span data-stu-id="b6d6b-103">uploadNewVersion action</span></span>

<span data-ttu-id="b6d6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6d6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6d6b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6d6b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6d6b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6d6b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6d6b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6d6b-108">Prerequisites</span></span>
<span data-ttu-id="b6d6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6d6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6d6b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6d6b-111">Permission type</span></span>|<span data-ttu-id="b6d6b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6d6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6d6b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6d6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6d6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6d6b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6d6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6d6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-116">Not supported.</span></span>|
|<span data-ttu-id="b6d6b-117">Application</span><span class="sxs-lookup"><span data-stu-id="b6d6b-117">Application</span></span>|<span data-ttu-id="b6d6b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d6b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6d6b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/uploadNewVersion
```

## <a name="request-headers"></a><span data-ttu-id="b6d6b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d6b-120">Request headers</span></span>
|<span data-ttu-id="b6d6b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6d6b-121">Header</span></span>|<span data-ttu-id="b6d6b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6d6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6d6b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6d6b-123">Authorization</span></span>|<span data-ttu-id="b6d6b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6d6b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6d6b-125">Accept</span></span>|<span data-ttu-id="b6d6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6d6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6d6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d6b-127">Request body</span></span>
<span data-ttu-id="b6d6b-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b6d6b-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b6d6b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6d6b-130">Property</span></span>|<span data-ttu-id="b6d6b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d6b-131">Type</span></span>|<span data-ttu-id="b6d6b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6d6b-133">content</span><span class="sxs-lookup"><span data-stu-id="b6d6b-133">content</span></span>|<span data-ttu-id="b6d6b-134">Binária</span><span class="sxs-lookup"><span data-stu-id="b6d6b-134">Binary</span></span>|<span data-ttu-id="b6d6b-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6d6b-135">Not yet documented</span></span>|
|<span data-ttu-id="b6d6b-136">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="b6d6b-136">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="b6d6b-137">coleção [groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="b6d6b-137">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="b6d6b-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6d6b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6d6b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d6b-139">Response</span></span>
<span data-ttu-id="b6d6b-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6d6b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6d6b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6d6b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d6b-142">Request</span></span>
<span data-ttu-id="b6d6b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/uploadNewVersion

Content-type: application/json
Content-length: 377

{
  "content": "Y29udGVudA==",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b6d6b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d6b-144">Response</span></span>
<span data-ttu-id="b6d6b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6d6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




