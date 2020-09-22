---
title: Listar iosUpdateConfigurations
description: Listar propriedades e relações dos objetos iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c53ea76fdac689374fc96b7abb7d24e12f3a277
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092143"
---
# <a name="list-iosupdateconfigurations"></a><span data-ttu-id="3b798-103">Listar iosUpdateConfigurations</span><span class="sxs-lookup"><span data-stu-id="3b798-103">List iosUpdateConfigurations</span></span>

<span data-ttu-id="3b798-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b798-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b798-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b798-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b798-106">Listar propriedades e relações dos objetos [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3b798-106">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b798-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b798-107">Prerequisites</span></span>
<span data-ttu-id="3b798-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b798-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b798-110">Permission type</span></span>|<span data-ttu-id="3b798-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b798-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b798-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b798-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b798-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b798-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3b798-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b798-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b798-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b798-115">Not supported.</span></span>|
|<span data-ttu-id="3b798-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b798-116">Application</span></span>|<span data-ttu-id="3b798-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b798-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b798-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b798-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3b798-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b798-119">Request headers</span></span>
|<span data-ttu-id="3b798-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b798-120">Header</span></span>|<span data-ttu-id="3b798-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b798-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b798-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b798-122">Authorization</span></span>|<span data-ttu-id="3b798-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b798-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b798-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b798-124">Accept</span></span>|<span data-ttu-id="3b798-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b798-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b798-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b798-126">Request body</span></span>
<span data-ttu-id="3b798-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b798-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b798-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b798-128">Response</span></span>
<span data-ttu-id="3b798-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b798-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b798-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b798-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b798-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b798-131">Request</span></span>
<span data-ttu-id="3b798-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b798-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3b798-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b798-133">Response</span></span>
<span data-ttu-id="3b798-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b798-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
      "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "activeHoursStart": "12:00:05.5020000",
      "activeHoursEnd": "11:59:00.8990000",
      "scheduledInstallDays": [
        "monday"
      ],
      "utcTimeOffsetInMinutes": 6
    }
  ]
}
```









