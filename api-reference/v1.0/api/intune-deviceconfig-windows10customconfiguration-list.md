---
title: Listar windows10CustomConfigurations
description: Listar propriedades e relações dos objetos windows10CustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebcf65e382e28e71b1564917143222ba00bd4cf4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365555"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="54fd7-103">Listar windows10CustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="54fd7-103">List windows10CustomConfigurations</span></span>

> <span data-ttu-id="54fd7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54fd7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54fd7-105">Listar propriedades e relações dos objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54fd7-105">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54fd7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54fd7-106">Prerequisites</span></span>
<span data-ttu-id="54fd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54fd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54fd7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54fd7-109">Permission type</span></span>|<span data-ttu-id="54fd7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54fd7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54fd7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54fd7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54fd7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="54fd7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="54fd7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54fd7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54fd7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54fd7-114">Not supported.</span></span>|
|<span data-ttu-id="54fd7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54fd7-115">Application</span></span>|<span data-ttu-id="54fd7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54fd7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54fd7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54fd7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54fd7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54fd7-118">Request headers</span></span>
|<span data-ttu-id="54fd7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54fd7-119">Header</span></span>|<span data-ttu-id="54fd7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="54fd7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54fd7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54fd7-121">Authorization</span></span>|<span data-ttu-id="54fd7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54fd7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54fd7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54fd7-123">Accept</span></span>|<span data-ttu-id="54fd7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="54fd7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54fd7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54fd7-125">Request body</span></span>
<span data-ttu-id="54fd7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54fd7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54fd7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="54fd7-127">Response</span></span>
<span data-ttu-id="54fd7-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54fd7-128">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54fd7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54fd7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="54fd7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54fd7-130">Request</span></span>
<span data-ttu-id="54fd7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54fd7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="54fd7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="54fd7-132">Response</span></span>
<span data-ttu-id="54fd7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54fd7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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




