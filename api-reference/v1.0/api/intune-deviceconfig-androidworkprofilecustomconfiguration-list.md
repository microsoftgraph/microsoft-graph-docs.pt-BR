---
title: Listar androidWorkProfileCustomConfigurations
description: Listar Propriedades e relações dos objetos androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 681028162c7e34f0108c061ef05d296e9d487f39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401228"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="60382-103">Listar androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="60382-103">List androidWorkProfileCustomConfigurations</span></span>

<span data-ttu-id="60382-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60382-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60382-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60382-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60382-106">Listar Propriedades e relações dos objetos [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="60382-106">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60382-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60382-107">Prerequisites</span></span>
<span data-ttu-id="60382-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60382-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60382-110">Permission type</span></span>|<span data-ttu-id="60382-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60382-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60382-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60382-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60382-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="60382-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="60382-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60382-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60382-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60382-115">Not supported.</span></span>|
|<span data-ttu-id="60382-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60382-116">Application</span></span>|<span data-ttu-id="60382-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60382-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60382-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60382-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="60382-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60382-119">Request headers</span></span>
|<span data-ttu-id="60382-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60382-120">Header</span></span>|<span data-ttu-id="60382-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60382-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60382-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60382-122">Authorization</span></span>|<span data-ttu-id="60382-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60382-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60382-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60382-124">Accept</span></span>|<span data-ttu-id="60382-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60382-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60382-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60382-126">Request body</span></span>
<span data-ttu-id="60382-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60382-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60382-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="60382-128">Response</span></span>
<span data-ttu-id="60382-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60382-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60382-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60382-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60382-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60382-131">Request</span></span>
<span data-ttu-id="60382-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60382-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="60382-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="60382-133">Response</span></span>
<span data-ttu-id="60382-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60382-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 682

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```






