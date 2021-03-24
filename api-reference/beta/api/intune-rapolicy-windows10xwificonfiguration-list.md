---
title: Listar windows10XWifiConfigurations
description: Listar propriedades e relações dos objetos windows10XWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 351c5ea0c72f82ba254d7672e10bbe96671c1529
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141635"
---
# <a name="list-windows10xwificonfigurations"></a><span data-ttu-id="952d9-103">Listar windows10XWifiConfigurations</span><span class="sxs-lookup"><span data-stu-id="952d9-103">List windows10XWifiConfigurations</span></span>

<span data-ttu-id="952d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="952d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="952d9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="952d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="952d9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="952d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="952d9-107">Listar propriedades e relações dos [objetos windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="952d9-107">List properties and relationships of the [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="952d9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="952d9-108">Prerequisites</span></span>
<span data-ttu-id="952d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="952d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="952d9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="952d9-111">Permission type</span></span>|<span data-ttu-id="952d9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="952d9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="952d9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="952d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="952d9-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="952d9-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="952d9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="952d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="952d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="952d9-116">Not supported.</span></span>|
|<span data-ttu-id="952d9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="952d9-117">Application</span></span>|<span data-ttu-id="952d9-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="952d9-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="952d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="952d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="952d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="952d9-120">Request headers</span></span>
|<span data-ttu-id="952d9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="952d9-121">Header</span></span>|<span data-ttu-id="952d9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="952d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="952d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="952d9-123">Authorization</span></span>|<span data-ttu-id="952d9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="952d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="952d9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="952d9-125">Accept</span></span>|<span data-ttu-id="952d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="952d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="952d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="952d9-127">Request body</span></span>
<span data-ttu-id="952d9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="952d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="952d9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="952d9-129">Response</span></span>
<span data-ttu-id="952d9-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="952d9-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="952d9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="952d9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="952d9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="952d9-132">Request</span></span>
<span data-ttu-id="952d9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="952d9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="952d9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="952d9-134">Response</span></span>
<span data-ttu-id="952d9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="952d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
      "id": "31063b86-3b86-3106-863b-0631863b0631",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
      "customXmlFileName": "Custom Xml File Name value",
      "customXml": "Y3VzdG9tWG1s"
    }
  ]
}
```




