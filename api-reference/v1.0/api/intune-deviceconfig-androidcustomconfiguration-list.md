---
title: Listar androidCustomConfigurations
description: Listar propriedades e relações dos objetos androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd078353e590b39afb8c010b9795d383f22ffd6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019657"
---
# <a name="list-androidcustomconfigurations"></a><span data-ttu-id="1c293-103">Listar androidCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="1c293-103">List androidCustomConfigurations</span></span>

> <span data-ttu-id="1c293-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c293-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c293-105">Listar propriedades e relações dos objetos [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c293-105">List properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c293-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c293-106">Prerequisites</span></span>
<span data-ttu-id="1c293-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c293-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c293-109">Permission type</span></span>|<span data-ttu-id="1c293-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c293-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c293-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c293-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c293-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c293-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c293-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c293-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c293-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c293-114">Not supported.</span></span>|
|<span data-ttu-id="1c293-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c293-115">Application</span></span>|<span data-ttu-id="1c293-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c293-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c293-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c293-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c293-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c293-118">Request headers</span></span>
|<span data-ttu-id="1c293-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c293-119">Header</span></span>|<span data-ttu-id="1c293-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1c293-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c293-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c293-121">Authorization</span></span>|<span data-ttu-id="1c293-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c293-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c293-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c293-123">Accept</span></span>|<span data-ttu-id="1c293-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c293-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c293-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c293-125">Request body</span></span>
<span data-ttu-id="1c293-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c293-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c293-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c293-127">Response</span></span>
<span data-ttu-id="1c293-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c293-128">If successful, this method returns a `200 OK` response code and a collection of [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c293-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c293-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c293-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c293-130">Request</span></span>
<span data-ttu-id="1c293-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c293-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1c293-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c293-132">Response</span></span>
<span data-ttu-id="1c293-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c293-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCustomConfiguration",
      "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



