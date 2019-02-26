---
title: Listar deviceConfigurations
description: Listar propriedades e relações dos objetos deviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19199da330a12ff400ee4b5845b8fcc580c35083
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257208"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="13ef5-103">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="13ef5-103">List deviceConfigurations</span></span>

> <span data-ttu-id="13ef5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13ef5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ef5-105">Listar propriedades e relações dos objetos [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13ef5-105">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13ef5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13ef5-106">Prerequisites</span></span>
<span data-ttu-id="13ef5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13ef5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13ef5-109">Permission type</span></span>|<span data-ttu-id="13ef5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13ef5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13ef5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13ef5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13ef5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13ef5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13ef5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13ef5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13ef5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13ef5-114">Not supported.</span></span>|
|<span data-ttu-id="13ef5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13ef5-115">Application</span></span>|<span data-ttu-id="13ef5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13ef5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13ef5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13ef5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13ef5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13ef5-118">Request headers</span></span>
|<span data-ttu-id="13ef5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13ef5-119">Header</span></span>|<span data-ttu-id="13ef5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="13ef5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13ef5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13ef5-121">Authorization</span></span>|<span data-ttu-id="13ef5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13ef5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13ef5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13ef5-123">Accept</span></span>|<span data-ttu-id="13ef5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13ef5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13ef5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13ef5-125">Request body</span></span>
<span data-ttu-id="13ef5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13ef5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13ef5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="13ef5-127">Response</span></span>
<span data-ttu-id="13ef5-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13ef5-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13ef5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13ef5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="13ef5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13ef5-130">Request</span></span>
<span data-ttu-id="13ef5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13ef5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="13ef5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="13ef5-132">Response</span></span>
<span data-ttu-id="13ef5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13ef5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfiguration",
      "id": "34977265-7265-3497-6572-973465729734",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



