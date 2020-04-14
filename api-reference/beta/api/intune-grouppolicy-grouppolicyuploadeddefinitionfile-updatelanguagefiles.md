---
title: ação updateLanguageFiles
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 631a147bf095930f12b729ae0ab79e01f1bffa91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440887"
---
# <a name="updatelanguagefiles-action"></a><span data-ttu-id="5134c-103">ação updateLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="5134c-103">updateLanguageFiles action</span></span>

<span data-ttu-id="5134c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5134c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5134c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5134c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5134c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5134c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5134c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5134c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5134c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5134c-108">Prerequisites</span></span>
<span data-ttu-id="5134c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5134c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5134c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5134c-111">Permission type</span></span>|<span data-ttu-id="5134c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5134c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5134c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5134c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5134c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5134c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5134c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5134c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5134c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5134c-116">Not supported.</span></span>|
|<span data-ttu-id="5134c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5134c-117">Application</span></span>|<span data-ttu-id="5134c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5134c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5134c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5134c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/updateLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="5134c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5134c-120">Request headers</span></span>
|<span data-ttu-id="5134c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5134c-121">Header</span></span>|<span data-ttu-id="5134c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5134c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5134c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5134c-123">Authorization</span></span>|<span data-ttu-id="5134c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5134c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5134c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5134c-125">Accept</span></span>|<span data-ttu-id="5134c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5134c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5134c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5134c-127">Request body</span></span>
<span data-ttu-id="5134c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5134c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5134c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="5134c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5134c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5134c-130">Property</span></span>|<span data-ttu-id="5134c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5134c-131">Type</span></span>|<span data-ttu-id="5134c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5134c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5134c-133">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="5134c-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="5134c-134">coleção [groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="5134c-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="5134c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5134c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5134c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5134c-136">Response</span></span>
<span data-ttu-id="5134c-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5134c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5134c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5134c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5134c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5134c-139">Request</span></span>
<span data-ttu-id="5134c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5134c-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/updateLanguageFiles

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

### <a name="response"></a><span data-ttu-id="5134c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5134c-141">Response</span></span>
<span data-ttu-id="5134c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5134c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



