---
title: Listar appleDeviceFeaturesConfigurationBases
description: Listar propriedades e relações dos objetos appleDeviceFeaturesConfigurationBase.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7b5d03e07730001deb4ecb7db9ce879cd16518c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515179"
---
# <a name="list-appledevicefeaturesconfigurationbases"></a><span data-ttu-id="13e16-103">Listar appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="13e16-103">List appleDeviceFeaturesConfigurationBases</span></span>

<span data-ttu-id="13e16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13e16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13e16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13e16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13e16-106">Listar propriedades e relações dos objetos [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="13e16-106">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13e16-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13e16-107">Prerequisites</span></span>
<span data-ttu-id="13e16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13e16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13e16-110">Permission type</span></span>|<span data-ttu-id="13e16-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13e16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13e16-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13e16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13e16-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13e16-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13e16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13e16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13e16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13e16-115">Not supported.</span></span>|
|<span data-ttu-id="13e16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13e16-116">Application</span></span>|<span data-ttu-id="13e16-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13e16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13e16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13e16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13e16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13e16-119">Request headers</span></span>
|<span data-ttu-id="13e16-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13e16-120">Header</span></span>|<span data-ttu-id="13e16-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13e16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13e16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13e16-122">Authorization</span></span>|<span data-ttu-id="13e16-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13e16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13e16-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13e16-124">Accept</span></span>|<span data-ttu-id="13e16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13e16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13e16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13e16-126">Request body</span></span>
<span data-ttu-id="13e16-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13e16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13e16-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="13e16-128">Response</span></span>
<span data-ttu-id="13e16-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13e16-129">If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13e16-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13e16-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13e16-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13e16-131">Request</span></span>
<span data-ttu-id="13e16-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13e16-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="13e16-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="13e16-133">Response</span></span>
<span data-ttu-id="13e16-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13e16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
      "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




