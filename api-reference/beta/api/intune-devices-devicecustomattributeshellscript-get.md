---
title: Obter deviceCustomAttributeShellScript
description: Leia as propriedades e as relações do objeto deviceCustomAttributeShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a72ba3b8c3fb379cd1177721f1c1503afc32d9c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212962"
---
# <a name="get-devicecustomattributeshellscript"></a><span data-ttu-id="72fa1-103">Obter deviceCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="72fa1-103">Get deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="72fa1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72fa1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72fa1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72fa1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72fa1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72fa1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72fa1-107">Leia as propriedades e as relações do objeto [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="72fa1-107">Read properties and relationships of the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72fa1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72fa1-108">Prerequisites</span></span>
<span data-ttu-id="72fa1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72fa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72fa1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72fa1-111">Permission type</span></span>|<span data-ttu-id="72fa1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72fa1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72fa1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72fa1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72fa1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="72fa1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="72fa1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72fa1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72fa1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72fa1-116">Not supported.</span></span>|
|<span data-ttu-id="72fa1-117">Application</span><span class="sxs-lookup"><span data-stu-id="72fa1-117">Application</span></span>|<span data-ttu-id="72fa1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="72fa1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72fa1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72fa1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72fa1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72fa1-120">Optional query parameters</span></span>
<span data-ttu-id="72fa1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72fa1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72fa1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72fa1-122">Request headers</span></span>
|<span data-ttu-id="72fa1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72fa1-123">Header</span></span>|<span data-ttu-id="72fa1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="72fa1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72fa1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72fa1-125">Authorization</span></span>|<span data-ttu-id="72fa1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72fa1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72fa1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72fa1-127">Accept</span></span>|<span data-ttu-id="72fa1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72fa1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72fa1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72fa1-129">Request body</span></span>
<span data-ttu-id="72fa1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72fa1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72fa1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="72fa1-131">Response</span></span>
<span data-ttu-id="72fa1-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72fa1-132">If successful, this method returns a `200 OK` response code and [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72fa1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72fa1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="72fa1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72fa1-134">Request</span></span>
<span data-ttu-id="72fa1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72fa1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

### <a name="response"></a><span data-ttu-id="72fa1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="72fa1-136">Response</span></span>
<span data-ttu-id="72fa1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72fa1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
    "id": "929d921b-921b-929d-1b92-9d921b929d92",
    "customAttributeName": "Custom Attribute Name value",
    "customAttributeType": "string",
    "displayName": "Display Name value",
    "description": "Description value",
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "fileName": "File Name value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




