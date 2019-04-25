---
title: Listar remoteActionAudits
description: Listar Propriedades e relações dos objetos remoteActionAudit.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b473ee244b289b5931776947749a73b06615b23
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523690"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="ea492-103">Listar remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="ea492-103">List remoteActionAudits</span></span>

> <span data-ttu-id="ea492-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea492-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea492-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea492-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea492-106">Listar Propriedades e relações dos objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="ea492-106">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea492-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea492-107">Prerequisites</span></span>
<span data-ttu-id="ea492-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea492-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea492-110">Permission type</span></span>|<span data-ttu-id="ea492-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea492-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea492-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea492-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea492-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea492-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ea492-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea492-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea492-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea492-115">Not supported.</span></span>|
|<span data-ttu-id="ea492-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea492-116">Application</span></span>|<span data-ttu-id="ea492-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea492-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea492-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea492-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="ea492-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea492-119">Request headers</span></span>
|<span data-ttu-id="ea492-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea492-120">Header</span></span>|<span data-ttu-id="ea492-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ea492-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea492-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea492-122">Authorization</span></span>|<span data-ttu-id="ea492-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea492-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea492-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea492-124">Accept</span></span>|<span data-ttu-id="ea492-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea492-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea492-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea492-126">Request body</span></span>
<span data-ttu-id="ea492-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea492-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea492-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea492-128">Response</span></span>
<span data-ttu-id="ea492-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea492-129">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea492-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea492-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea492-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea492-131">Request</span></span>
<span data-ttu-id="ea492-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea492-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="ea492-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea492-133">Response</span></span>
<span data-ttu-id="ea492-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea492-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





