---
title: função getTopMobileApps
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68646ead33d9505522381ace92e5eeaa3e7b48ce
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974234"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="218f2-103">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="218f2-103">getTopMobileApps function</span></span>

> <span data-ttu-id="218f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="218f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="218f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="218f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="218f2-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="218f2-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="218f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="218f2-107">Prerequisites</span></span>
<span data-ttu-id="218f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="218f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="218f2-110">Permission type</span></span>|<span data-ttu-id="218f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="218f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="218f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="218f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="218f2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="218f2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="218f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="218f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="218f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="218f2-115">Not supported.</span></span>|
|<span data-ttu-id="218f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="218f2-116">Application</span></span>|<span data-ttu-id="218f2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="218f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="218f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="218f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="218f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="218f2-119">Request headers</span></span>
|<span data-ttu-id="218f2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="218f2-120">Header</span></span>|<span data-ttu-id="218f2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="218f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="218f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="218f2-122">Authorization</span></span>|<span data-ttu-id="218f2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="218f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="218f2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="218f2-124">Accept</span></span>|<span data-ttu-id="218f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="218f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="218f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="218f2-126">Request body</span></span>
<span data-ttu-id="218f2-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="218f2-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="218f2-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="218f2-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="218f2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="218f2-129">Property</span></span>|<span data-ttu-id="218f2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="218f2-130">Type</span></span>|<span data-ttu-id="218f2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="218f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="218f2-132">status</span><span class="sxs-lookup"><span data-stu-id="218f2-132">status</span></span>|<span data-ttu-id="218f2-133">String</span><span class="sxs-lookup"><span data-stu-id="218f2-133">String</span></span>|<span data-ttu-id="218f2-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="218f2-134">Not yet documented</span></span>|
|<span data-ttu-id="218f2-135">Count</span><span class="sxs-lookup"><span data-stu-id="218f2-135">count</span></span>|<span data-ttu-id="218f2-136">Int64</span><span class="sxs-lookup"><span data-stu-id="218f2-136">Int64</span></span>|<span data-ttu-id="218f2-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="218f2-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="218f2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="218f2-138">Response</span></span>
<span data-ttu-id="218f2-139">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileApp](../resources/intune-apps-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="218f2-139">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="218f2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="218f2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="218f2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="218f2-141">Request</span></span>
<span data-ttu-id="218f2-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="218f2-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="218f2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="218f2-143">Response</span></span>
<span data-ttu-id="218f2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="218f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

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
      ]
    }
  ]
}
```




