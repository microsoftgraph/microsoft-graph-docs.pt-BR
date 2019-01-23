---
title: Obter deviceConfigurationConflictSummary
description: Leia as propriedades e os relacionamentos do objeto deviceConfigurationConflictSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 47ce8bd580817bb03fa6f5775a98296f447830ed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408359"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="c4d16-103">Obter deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="c4d16-103">Get deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="c4d16-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c4d16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4d16-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c4d16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4d16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c4d16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4d16-107">Leia as propriedades e os relacionamentos do objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c4d16-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4d16-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4d16-108">Prerequisites</span></span>
<span data-ttu-id="c4d16-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4d16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4d16-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4d16-111">Permission type</span></span>|<span data-ttu-id="c4d16-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4d16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4d16-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4d16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4d16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4d16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c4d16-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4d16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4d16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4d16-116">Not supported.</span></span>|
|<span data-ttu-id="c4d16-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4d16-117">Application</span></span>|<span data-ttu-id="c4d16-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4d16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4d16-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4d16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4d16-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4d16-120">Optional query parameters</span></span>
<span data-ttu-id="c4d16-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4d16-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4d16-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d16-122">Request headers</span></span>
|<span data-ttu-id="c4d16-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4d16-123">Header</span></span>|<span data-ttu-id="c4d16-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c4d16-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4d16-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4d16-125">Authorization</span></span>|<span data-ttu-id="c4d16-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4d16-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4d16-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4d16-127">Accept</span></span>|<span data-ttu-id="c4d16-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c4d16-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4d16-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d16-129">Request body</span></span>
<span data-ttu-id="c4d16-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4d16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4d16-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4d16-131">Response</span></span>
<span data-ttu-id="c4d16-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4d16-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4d16-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4d16-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4d16-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d16-134">Request</span></span>
<span data-ttu-id="c4d16-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4d16-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="c4d16-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4d16-136">Response</span></span>
<span data-ttu-id="c4d16-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4d16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value"
      }
    ],
    "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
    "contributingSettings": [
      "Contributing Settings value"
    ],
    "deviceCheckinsImpacted": 6
  }
}
```




