---
title: Listar appleDeviceFeaturesConfigurationBases
description: Listar propriedades e relações dos objetos appleDeviceFeaturesConfigurationBase.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12c100d1b0dae11f07901dec979dfdf9425cd87e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257047"
---
# <a name="list-appledevicefeaturesconfigurationbases"></a><span data-ttu-id="9e027-103">Listar appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="9e027-103">List appleDeviceFeaturesConfigurationBases</span></span>

> <span data-ttu-id="9e027-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e027-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e027-105">Listar propriedades e relações dos objetos [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="9e027-105">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e027-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e027-106">Prerequisites</span></span>
<span data-ttu-id="9e027-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e027-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e027-109">Permission type</span></span>|<span data-ttu-id="9e027-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e027-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e027-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e027-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e027-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e027-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e027-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e027-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e027-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e027-114">Not supported.</span></span>|
|<span data-ttu-id="9e027-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e027-115">Application</span></span>|<span data-ttu-id="9e027-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e027-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e027-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e027-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e027-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e027-118">Request headers</span></span>
|<span data-ttu-id="9e027-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e027-119">Header</span></span>|<span data-ttu-id="9e027-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9e027-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e027-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e027-121">Authorization</span></span>|<span data-ttu-id="9e027-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e027-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e027-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e027-123">Accept</span></span>|<span data-ttu-id="9e027-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e027-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e027-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e027-125">Request body</span></span>
<span data-ttu-id="9e027-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e027-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e027-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e027-127">Response</span></span>
<span data-ttu-id="9e027-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e027-128">If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e027-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e027-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e027-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e027-130">Request</span></span>
<span data-ttu-id="9e027-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e027-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9e027-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e027-132">Response</span></span>
<span data-ttu-id="9e027-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e027-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



