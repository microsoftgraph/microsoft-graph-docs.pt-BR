---
title: função getTopMobileApps
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd77e9ef52131844f46f4551e882f289ebcc345f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800778"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="dec37-103">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="dec37-103">getTopMobileApps function</span></span>

> <span data-ttu-id="dec37-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dec37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dec37-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dec37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dec37-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dec37-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dec37-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dec37-107">Prerequisites</span></span>
<span data-ttu-id="dec37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec37-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dec37-110">Permission type</span></span>|<span data-ttu-id="dec37-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dec37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dec37-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dec37-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dec37-113">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="dec37-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="dec37-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dec37-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dec37-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dec37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dec37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dec37-116">Not supported.</span></span>|
|<span data-ttu-id="dec37-117">Application</span><span class="sxs-lookup"><span data-stu-id="dec37-117">Application</span></span>||
| <span data-ttu-id="dec37-118">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="dec37-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="dec37-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dec37-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dec37-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dec37-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dec37-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dec37-121">Request headers</span></span>
|<span data-ttu-id="dec37-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dec37-122">Header</span></span>|<span data-ttu-id="dec37-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dec37-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dec37-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dec37-124">Authorization</span></span>|<span data-ttu-id="dec37-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dec37-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dec37-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dec37-126">Accept</span></span>|<span data-ttu-id="dec37-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dec37-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dec37-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dec37-128">Request body</span></span>
<span data-ttu-id="dec37-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="dec37-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="dec37-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="dec37-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="dec37-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dec37-131">Property</span></span>|<span data-ttu-id="dec37-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="dec37-132">Type</span></span>|<span data-ttu-id="dec37-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="dec37-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec37-134">status</span><span class="sxs-lookup"><span data-stu-id="dec37-134">status</span></span>|<span data-ttu-id="dec37-135">String</span><span class="sxs-lookup"><span data-stu-id="dec37-135">String</span></span>|<span data-ttu-id="dec37-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dec37-136">Not yet documented</span></span>|
|<span data-ttu-id="dec37-137">count</span><span class="sxs-lookup"><span data-stu-id="dec37-137">count</span></span>|<span data-ttu-id="dec37-138">Int64</span><span class="sxs-lookup"><span data-stu-id="dec37-138">Int64</span></span>|<span data-ttu-id="dec37-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dec37-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dec37-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dec37-140">Response</span></span>
<span data-ttu-id="dec37-141">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dec37-141">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dec37-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dec37-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="dec37-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dec37-143">Request</span></span>
<span data-ttu-id="dec37-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dec37-144">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="dec37-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dec37-145">Response</span></span>
<span data-ttu-id="dec37-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dec37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1
    }
  ]
}
```







