---
title: Obter Propriedadesdeviceconfigurationconflictsummary
description: Leia as propriedades e as relações do objeto Propriedadesdeviceconfigurationconflictsummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c2bffcd19b7a5527e2a0a775c4a30b29ec6ac33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291754"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="8d405-103">Obter Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="8d405-103">Get deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="8d405-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d405-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d405-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d405-107">Leia as propriedades e as relações do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8d405-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d405-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d405-108">Prerequisites</span></span>
<span data-ttu-id="8d405-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d405-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d405-111">Permission type</span></span>|<span data-ttu-id="8d405-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d405-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d405-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d405-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d405-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d405-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d405-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d405-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d405-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d405-116">Not supported.</span></span>|
|<span data-ttu-id="8d405-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d405-117">Application</span></span>|<span data-ttu-id="8d405-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d405-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d405-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d405-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d405-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d405-120">Optional query parameters</span></span>
<span data-ttu-id="8d405-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d405-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d405-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d405-122">Request headers</span></span>
|<span data-ttu-id="8d405-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d405-123">Header</span></span>|<span data-ttu-id="8d405-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8d405-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d405-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d405-125">Authorization</span></span>|<span data-ttu-id="8d405-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d405-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d405-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d405-127">Accept</span></span>|<span data-ttu-id="8d405-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8d405-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d405-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d405-129">Request body</span></span>
<span data-ttu-id="8d405-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d405-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d405-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d405-131">Response</span></span>
<span data-ttu-id="8d405-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d405-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d405-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d405-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d405-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d405-134">Request</span></span>
<span data-ttu-id="8d405-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d405-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="8d405-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d405-136">Response</span></span>
<span data-ttu-id="8d405-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d405-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value",
        "sourceType": "deviceIntent"
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




