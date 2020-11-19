---
title: ação removeLanguageFiles
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30b1d7e06d69b768fd954a82b3ae3925cd274b42
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224708"
---
# <a name="removelanguagefiles-action"></a><span data-ttu-id="78e83-103">ação removeLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="78e83-103">removeLanguageFiles action</span></span>

<span data-ttu-id="78e83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78e83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78e83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78e83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e83-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="78e83-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78e83-108">Prerequisites</span></span>
<span data-ttu-id="78e83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78e83-111">Permission type</span></span>|<span data-ttu-id="78e83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78e83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e83-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78e83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78e83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78e83-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78e83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78e83-116">Not supported.</span></span>|
|<span data-ttu-id="78e83-117">Application</span><span class="sxs-lookup"><span data-stu-id="78e83-117">Application</span></span>|<span data-ttu-id="78e83-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e83-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78e83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/removeLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="78e83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78e83-120">Request headers</span></span>
|<span data-ttu-id="78e83-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78e83-121">Header</span></span>|<span data-ttu-id="78e83-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78e83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78e83-123">Authorization</span></span>|<span data-ttu-id="78e83-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78e83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e83-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78e83-125">Accept</span></span>|<span data-ttu-id="78e83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78e83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78e83-127">Request body</span></span>
<span data-ttu-id="78e83-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="78e83-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="78e83-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="78e83-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="78e83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78e83-130">Property</span></span>|<span data-ttu-id="78e83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78e83-131">Type</span></span>|<span data-ttu-id="78e83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e83-133">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="78e83-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="78e83-134">coleção [groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="78e83-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="78e83-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="78e83-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="78e83-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e83-136">Response</span></span>
<span data-ttu-id="78e83-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="78e83-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="78e83-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78e83-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e83-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78e83-139">Request</span></span>
<span data-ttu-id="78e83-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78e83-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/removeLanguageFiles

Content-type: application/json
Content-length: 347

{
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

### <a name="response"></a><span data-ttu-id="78e83-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e83-141">Response</span></span>
<span data-ttu-id="78e83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78e83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




