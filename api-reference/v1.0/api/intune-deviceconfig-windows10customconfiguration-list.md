---
title: Listar windows10CustomConfigurations
description: Listar propriedades e relações dos objetos windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe429488befef4c727bfd915a97dcea5dd179b4e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756201"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="b2e01-103">Listar windows10CustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="b2e01-103">List windows10CustomConfigurations</span></span>

<span data-ttu-id="b2e01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2e01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2e01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2e01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e01-106">Listar propriedades e relações dos objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2e01-106">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2e01-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2e01-107">Prerequisites</span></span>
<span data-ttu-id="b2e01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2e01-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2e01-110">Permission type</span></span>|<span data-ttu-id="b2e01-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2e01-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2e01-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2e01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2e01-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2e01-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2e01-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2e01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2e01-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2e01-115">Not supported.</span></span>|
|<span data-ttu-id="b2e01-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2e01-116">Application</span></span>|<span data-ttu-id="b2e01-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2e01-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2e01-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2e01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b2e01-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e01-119">Request headers</span></span>
|<span data-ttu-id="b2e01-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2e01-120">Header</span></span>|<span data-ttu-id="b2e01-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2e01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2e01-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2e01-122">Authorization</span></span>|<span data-ttu-id="b2e01-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2e01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2e01-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2e01-124">Accept</span></span>|<span data-ttu-id="b2e01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2e01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2e01-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e01-126">Request body</span></span>
<span data-ttu-id="b2e01-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2e01-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2e01-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2e01-128">Response</span></span>
<span data-ttu-id="b2e01-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2e01-129">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2e01-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2e01-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2e01-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e01-131">Request</span></span>
<span data-ttu-id="b2e01-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2e01-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b2e01-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2e01-133">Response</span></span>
<span data-ttu-id="b2e01-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2e01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 643

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
          "@odata.type": "microsoft.graph.omaSetting",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value"
        }
      ]
    }
  ]
}
```




