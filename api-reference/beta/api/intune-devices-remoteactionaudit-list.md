---
title: Lista remoteActionAudits
description: Lista as propriedades e os relacionamentos dos objetos remoteActionAudit.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8124c5da95e01c1c0513e5f8ac88cd45d7943fd5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971169"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="cb3cb-103">Lista remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="cb3cb-103">List remoteActionAudits</span></span>

> <span data-ttu-id="cb3cb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb3cb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb3cb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb3cb-107">Lista as propriedades e os relacionamentos dos objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="cb3cb-107">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb3cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb3cb-108">Prerequisites</span></span>
<span data-ttu-id="cb3cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb3cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb3cb-111">Permission type</span></span>|<span data-ttu-id="cb3cb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb3cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb3cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb3cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb3cb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb3cb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cb3cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb3cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb3cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-116">Not supported.</span></span>|
|<span data-ttu-id="cb3cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb3cb-117">Application</span></span>|<span data-ttu-id="cb3cb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb3cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="cb3cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3cb-120">Request headers</span></span>
|<span data-ttu-id="cb3cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb3cb-121">Header</span></span>|<span data-ttu-id="cb3cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cb3cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb3cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb3cb-123">Authorization</span></span>|<span data-ttu-id="cb3cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb3cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb3cb-125">Accept</span></span>|<span data-ttu-id="cb3cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb3cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3cb-127">Request body</span></span>
<span data-ttu-id="cb3cb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb3cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb3cb-129">Response</span></span>
<span data-ttu-id="cb3cb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-130">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb3cb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb3cb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb3cb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3cb-132">Request</span></span>
<span data-ttu-id="cb3cb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="cb3cb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb3cb-134">Response</span></span>
<span data-ttu-id="cb3cb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb3cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteActionAudit",
      "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
      "action": "factoryReset",
      "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
      "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
      "deviceIMEI": "Device IMEI value",
      "actionState": "pending"
    }
  ]
}
```





