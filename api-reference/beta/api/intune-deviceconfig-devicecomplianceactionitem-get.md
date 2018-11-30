---
title: Acessar deviceComplianceActionItem
description: Leia as propriedades e as relações do objeto deviceComplianceActionItem.
ms.openlocfilehash: 3575a137d3f08cf50684a82d00587a35e601c45b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034874"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="d4941-103">Acessar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="d4941-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="d4941-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4941-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4941-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4941-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4941-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d4941-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4941-107">Leia as propriedades e as relações do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="d4941-107">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4941-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4941-108">Prerequisites</span></span>
<span data-ttu-id="d4941-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4941-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4941-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4941-111">Permission type</span></span>|<span data-ttu-id="d4941-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4941-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4941-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4941-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4941-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4941-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d4941-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4941-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4941-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4941-116">Not supported.</span></span>|
|<span data-ttu-id="d4941-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4941-117">Application</span></span>|<span data-ttu-id="d4941-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4941-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4941-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4941-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4941-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4941-120">Optional query parameters</span></span>
<span data-ttu-id="d4941-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4941-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d4941-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4941-122">Request headers</span></span>
|<span data-ttu-id="d4941-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4941-123">Header</span></span>|<span data-ttu-id="d4941-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d4941-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4941-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4941-125">Authorization</span></span>|<span data-ttu-id="d4941-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4941-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4941-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d4941-127">Accept</span></span>|<span data-ttu-id="d4941-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d4941-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4941-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4941-129">Request body</span></span>
<span data-ttu-id="d4941-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4941-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4941-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4941-131">Response</span></span>
<span data-ttu-id="d4941-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4941-132">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4941-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4941-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4941-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4941-134">Request</span></span>
<span data-ttu-id="d4941-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4941-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="d4941-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4941-136">Response</span></span>
<span data-ttu-id="d4941-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4941-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
    "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
    "gracePeriodHours": 0,
    "actionType": "notification",
    "notificationTemplateId": "Notification Template Id value",
    "notificationMessageCCList": [
      "Notification Message CCList value"
    ]
  }
}
```





