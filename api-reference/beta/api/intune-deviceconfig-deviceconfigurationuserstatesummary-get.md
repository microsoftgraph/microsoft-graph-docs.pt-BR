---
title: Obter deviceConfigurationUserStateSummary
description: Leia as propriedades e as relações do objeto deviceConfigurationUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9019c9ab59bdd1a1f7ec21d987032410a7e8e15d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291482"
---
# <a name="get-deviceconfigurationuserstatesummary"></a><span data-ttu-id="0794c-103">Obter deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="0794c-103">Get deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="0794c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0794c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0794c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0794c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0794c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0794c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0794c-107">Leia as propriedades e as relações do objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0794c-107">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0794c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0794c-108">Prerequisites</span></span>
<span data-ttu-id="0794c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0794c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0794c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0794c-111">Permission type</span></span>|<span data-ttu-id="0794c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0794c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0794c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0794c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0794c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0794c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0794c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0794c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0794c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0794c-116">Not supported.</span></span>|
|<span data-ttu-id="0794c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0794c-117">Application</span></span>|<span data-ttu-id="0794c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0794c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0794c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0794c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0794c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0794c-120">Optional query parameters</span></span>
<span data-ttu-id="0794c-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0794c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0794c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0794c-122">Request headers</span></span>
|<span data-ttu-id="0794c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0794c-123">Header</span></span>|<span data-ttu-id="0794c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0794c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0794c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0794c-125">Authorization</span></span>|<span data-ttu-id="0794c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0794c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0794c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0794c-127">Accept</span></span>|<span data-ttu-id="0794c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0794c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0794c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0794c-129">Request body</span></span>
<span data-ttu-id="0794c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0794c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0794c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0794c-131">Response</span></span>
<span data-ttu-id="0794c-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0794c-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0794c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0794c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0794c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0794c-134">Request</span></span>
<span data-ttu-id="0794c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0794c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
```

### <a name="response"></a><span data-ttu-id="0794c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0794c-136">Response</span></span>
<span data-ttu-id="0794c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0794c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 361

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
    "id": "e8957887-7887-e895-8778-95e8877895e8",
    "unknownUserCount": 0,
    "notApplicableUserCount": 6,
    "compliantUserCount": 2,
    "remediatedUserCount": 3,
    "nonCompliantUserCount": 5,
    "errorUserCount": 14,
    "conflictUserCount": 1
  }
}
```




