---
title: Listar windows10EnterpriseModernAppManagementConfigurations
description: Listar propriedades e relações dos objetos windows10EnterpriseModernAppManagementConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80043a4f1073613df34181cecec4b0942a81d347
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758161"
---
# <a name="list-windows10enterprisemodernappmanagementconfigurations"></a><span data-ttu-id="8829f-103">Listar windows10EnterpriseModernAppManagementConfigurations</span><span class="sxs-lookup"><span data-stu-id="8829f-103">List windows10EnterpriseModernAppManagementConfigurations</span></span>

<span data-ttu-id="8829f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8829f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8829f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8829f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8829f-106">Listar propriedades e relações dos objetos [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8829f-106">List properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8829f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8829f-107">Prerequisites</span></span>
<span data-ttu-id="8829f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8829f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8829f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8829f-110">Permission type</span></span>|<span data-ttu-id="8829f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8829f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8829f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8829f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8829f-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8829f-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8829f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8829f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8829f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8829f-115">Not supported.</span></span>|
|<span data-ttu-id="8829f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8829f-116">Application</span></span>|<span data-ttu-id="8829f-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8829f-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8829f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8829f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8829f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8829f-119">Request headers</span></span>
|<span data-ttu-id="8829f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8829f-120">Header</span></span>|<span data-ttu-id="8829f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8829f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8829f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8829f-122">Authorization</span></span>|<span data-ttu-id="8829f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8829f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8829f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8829f-124">Accept</span></span>|<span data-ttu-id="8829f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8829f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8829f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8829f-126">Request body</span></span>
<span data-ttu-id="8829f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8829f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8829f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8829f-128">Response</span></span>
<span data-ttu-id="8829f-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8829f-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8829f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8829f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8829f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8829f-131">Request</span></span>
<span data-ttu-id="8829f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8829f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8829f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8829f-133">Response</span></span>
<span data-ttu-id="8829f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8829f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
      "id": "d6577687-7687-d657-8776-57d6877657d6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "uninstallBuiltInApps": true
    }
  ]
}
```




