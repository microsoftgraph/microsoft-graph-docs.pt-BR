---
title: ação removeLanguageFiles
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1d8945d36c5860695019c203869da0fd09b0043
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726609"
---
# <a name="removelanguagefiles-action"></a><span data-ttu-id="cbde6-103">ação removeLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="cbde6-103">removeLanguageFiles action</span></span>

<span data-ttu-id="cbde6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbde6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbde6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cbde6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbde6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbde6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbde6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cbde6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbde6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbde6-108">Prerequisites</span></span>
<span data-ttu-id="cbde6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbde6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbde6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbde6-111">Permission type</span></span>|<span data-ttu-id="cbde6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbde6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbde6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbde6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbde6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbde6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cbde6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbde6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbde6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbde6-116">Not supported.</span></span>|
|<span data-ttu-id="cbde6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbde6-117">Application</span></span>|<span data-ttu-id="cbde6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbde6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbde6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbde6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/removeLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="cbde6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbde6-120">Request headers</span></span>
|<span data-ttu-id="cbde6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbde6-121">Header</span></span>|<span data-ttu-id="cbde6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cbde6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbde6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbde6-123">Authorization</span></span>|<span data-ttu-id="cbde6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbde6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbde6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbde6-125">Accept</span></span>|<span data-ttu-id="cbde6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbde6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbde6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbde6-127">Request body</span></span>
<span data-ttu-id="cbde6-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="cbde6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cbde6-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="cbde6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cbde6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbde6-130">Property</span></span>|<span data-ttu-id="cbde6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbde6-131">Type</span></span>|<span data-ttu-id="cbde6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbde6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbde6-133">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="cbde6-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="cbde6-134">coleção [groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="cbde6-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="cbde6-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cbde6-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cbde6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbde6-136">Response</span></span>
<span data-ttu-id="cbde6-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cbde6-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cbde6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbde6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbde6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbde6-139">Request</span></span>
<span data-ttu-id="cbde6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbde6-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cbde6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbde6-141">Response</span></span>
<span data-ttu-id="cbde6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbde6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





