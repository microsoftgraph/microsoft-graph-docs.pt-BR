---
title: função getTopMobileApps
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc5697df9862ce1b17361ba3ec6b5b9c0a573463
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053843"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="408a7-103">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="408a7-103">getTopMobileApps function</span></span>

<span data-ttu-id="408a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="408a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="408a7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="408a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="408a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="408a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="408a7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="408a7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="408a7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="408a7-108">Prerequisites</span></span>
<span data-ttu-id="408a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="408a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="408a7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="408a7-111">Permission type</span></span>|<span data-ttu-id="408a7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="408a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="408a7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="408a7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="408a7-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="408a7-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="408a7-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="408a7-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="408a7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="408a7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="408a7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="408a7-117">Not supported.</span></span>|
|<span data-ttu-id="408a7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="408a7-118">Application</span></span>||
| <span data-ttu-id="408a7-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="408a7-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="408a7-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="408a7-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="408a7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="408a7-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="408a7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="408a7-122">Request headers</span></span>
|<span data-ttu-id="408a7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="408a7-123">Header</span></span>|<span data-ttu-id="408a7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="408a7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="408a7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="408a7-125">Authorization</span></span>|<span data-ttu-id="408a7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="408a7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="408a7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="408a7-127">Accept</span></span>|<span data-ttu-id="408a7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="408a7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="408a7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="408a7-129">Request body</span></span>
<span data-ttu-id="408a7-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="408a7-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="408a7-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="408a7-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="408a7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="408a7-132">Property</span></span>|<span data-ttu-id="408a7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="408a7-133">Type</span></span>|<span data-ttu-id="408a7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="408a7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="408a7-135">status</span><span class="sxs-lookup"><span data-stu-id="408a7-135">status</span></span>|<span data-ttu-id="408a7-136">String</span><span class="sxs-lookup"><span data-stu-id="408a7-136">String</span></span>|<span data-ttu-id="408a7-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="408a7-137">Not yet documented</span></span>|
|<span data-ttu-id="408a7-138">count</span><span class="sxs-lookup"><span data-stu-id="408a7-138">count</span></span>|<span data-ttu-id="408a7-139">Int64</span><span class="sxs-lookup"><span data-stu-id="408a7-139">Int64</span></span>|<span data-ttu-id="408a7-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="408a7-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="408a7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="408a7-141">Response</span></span>
<span data-ttu-id="408a7-142">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="408a7-142">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="408a7-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="408a7-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="408a7-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="408a7-144">Request</span></span>
<span data-ttu-id="408a7-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="408a7-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="408a7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="408a7-146">Response</span></span>
<span data-ttu-id="408a7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="408a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









