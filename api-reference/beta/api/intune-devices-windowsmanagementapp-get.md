---
title: Obter windowsManagementApp
description: Leia as propriedades e as relações do objeto windowsManagementApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5524ddba642db143b53e417b01f430a9c57d1ff8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43321615"
---
# <a name="get-windowsmanagementapp"></a><span data-ttu-id="2bf02-103">Obter windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="2bf02-103">Get windowsManagementApp</span></span>

<span data-ttu-id="2bf02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bf02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bf02-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bf02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bf02-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bf02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bf02-107">Leia as propriedades e as relações do objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2bf02-107">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bf02-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bf02-108">Prerequisites</span></span>
<span data-ttu-id="2bf02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bf02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bf02-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bf02-111">Permission type</span></span>|<span data-ttu-id="2bf02-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bf02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bf02-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bf02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bf02-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bf02-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2bf02-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bf02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bf02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bf02-116">Not supported.</span></span>|
|<span data-ttu-id="2bf02-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bf02-117">Application</span></span>|<span data-ttu-id="2bf02-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bf02-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bf02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bf02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2bf02-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bf02-120">Optional query parameters</span></span>
<span data-ttu-id="2bf02-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2bf02-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bf02-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf02-122">Request headers</span></span>
|<span data-ttu-id="2bf02-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bf02-123">Header</span></span>|<span data-ttu-id="2bf02-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2bf02-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bf02-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bf02-125">Authorization</span></span>|<span data-ttu-id="2bf02-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bf02-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bf02-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bf02-127">Accept</span></span>|<span data-ttu-id="2bf02-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2bf02-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bf02-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf02-129">Request body</span></span>
<span data-ttu-id="2bf02-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bf02-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bf02-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf02-131">Response</span></span>
<span data-ttu-id="2bf02-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bf02-132">If successful, this method returns a `200 OK` response code and [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bf02-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bf02-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bf02-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf02-134">Request</span></span>
<span data-ttu-id="2bf02-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bf02-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
```

### <a name="response"></a><span data-ttu-id="2bf02-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf02-136">Response</span></span>
<span data-ttu-id="2bf02-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bf02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementApp",
    "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
    "availableVersion": "Available Version value"
  }
}
```



