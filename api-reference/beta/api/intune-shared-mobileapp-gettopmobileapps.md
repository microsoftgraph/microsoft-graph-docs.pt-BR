---
title: Função getTopMobileApps
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 426d79529414bd44f0a2327d503adf388943aaf5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865905"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="ff225-103">Função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="ff225-103">getTopMobileApps function</span></span>

<span data-ttu-id="ff225-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff225-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff225-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff225-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff225-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff225-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff225-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff225-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff225-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff225-108">Prerequisites</span></span>
<span data-ttu-id="ff225-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff225-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff225-111">Permission type</span></span>|<span data-ttu-id="ff225-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff225-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff225-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff225-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ff225-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="ff225-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ff225-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff225-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ff225-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff225-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff225-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff225-117">Not supported.</span></span>|
|<span data-ttu-id="ff225-118">Application</span><span class="sxs-lookup"><span data-stu-id="ff225-118">Application</span></span>||
| <span data-ttu-id="ff225-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="ff225-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ff225-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff225-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff225-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff225-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ff225-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff225-122">Request headers</span></span>
|<span data-ttu-id="ff225-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff225-123">Header</span></span>|<span data-ttu-id="ff225-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ff225-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff225-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff225-125">Authorization</span></span>|<span data-ttu-id="ff225-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff225-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff225-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff225-127">Accept</span></span>|<span data-ttu-id="ff225-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff225-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff225-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff225-129">Request body</span></span>
<span data-ttu-id="ff225-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="ff225-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ff225-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="ff225-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ff225-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff225-132">Property</span></span>|<span data-ttu-id="ff225-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff225-133">Type</span></span>|<span data-ttu-id="ff225-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff225-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff225-135">status</span><span class="sxs-lookup"><span data-stu-id="ff225-135">status</span></span>|<span data-ttu-id="ff225-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff225-136">String</span></span>|<span data-ttu-id="ff225-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff225-137">Not yet documented</span></span>|
|<span data-ttu-id="ff225-138">count</span><span class="sxs-lookup"><span data-stu-id="ff225-138">count</span></span>|<span data-ttu-id="ff225-139">Int64</span><span class="sxs-lookup"><span data-stu-id="ff225-139">Int64</span></span>|<span data-ttu-id="ff225-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff225-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff225-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff225-141">Response</span></span>
<span data-ttu-id="ff225-142">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff225-142">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff225-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff225-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff225-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff225-144">Request</span></span>
<span data-ttu-id="ff225-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff225-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="ff225-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff225-146">Response</span></span>
<span data-ttu-id="ff225-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff225-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







