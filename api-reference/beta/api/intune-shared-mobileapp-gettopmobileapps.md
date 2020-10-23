---
title: função getTopMobileApps
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce107870a7839c3a8707819f2714dc38be2c6da9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735341"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="eb642-103">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="eb642-103">getTopMobileApps function</span></span>

<span data-ttu-id="eb642-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb642-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb642-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb642-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb642-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb642-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb642-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eb642-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb642-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb642-108">Prerequisites</span></span>
<span data-ttu-id="eb642-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb642-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb642-111">Permission type</span></span>|<span data-ttu-id="eb642-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb642-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb642-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb642-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eb642-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="eb642-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="eb642-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb642-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb642-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb642-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb642-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb642-117">Not supported.</span></span>|
|<span data-ttu-id="eb642-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb642-118">Application</span></span>||
| <span data-ttu-id="eb642-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="eb642-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="eb642-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb642-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb642-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb642-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="eb642-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb642-122">Request headers</span></span>
|<span data-ttu-id="eb642-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb642-123">Header</span></span>|<span data-ttu-id="eb642-124">Valor</span><span class="sxs-lookup"><span data-stu-id="eb642-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb642-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb642-125">Authorization</span></span>|<span data-ttu-id="eb642-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb642-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb642-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb642-127">Accept</span></span>|<span data-ttu-id="eb642-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eb642-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb642-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb642-129">Request body</span></span>
<span data-ttu-id="eb642-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="eb642-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="eb642-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="eb642-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="eb642-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb642-132">Property</span></span>|<span data-ttu-id="eb642-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb642-133">Type</span></span>|<span data-ttu-id="eb642-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb642-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb642-135">status</span><span class="sxs-lookup"><span data-stu-id="eb642-135">status</span></span>|<span data-ttu-id="eb642-136">String</span><span class="sxs-lookup"><span data-stu-id="eb642-136">String</span></span>|<span data-ttu-id="eb642-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eb642-137">Not yet documented</span></span>|
|<span data-ttu-id="eb642-138">count</span><span class="sxs-lookup"><span data-stu-id="eb642-138">count</span></span>|<span data-ttu-id="eb642-139">Int64</span><span class="sxs-lookup"><span data-stu-id="eb642-139">Int64</span></span>|<span data-ttu-id="eb642-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eb642-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eb642-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb642-141">Response</span></span>
<span data-ttu-id="eb642-142">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb642-142">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb642-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb642-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb642-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb642-144">Request</span></span>
<span data-ttu-id="eb642-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb642-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="eb642-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb642-146">Response</span></span>
<span data-ttu-id="eb642-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb642-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








