---
title: Get deviceAppManagement
description: Ler propriedades e relações do objeto deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db41690238511e9e36f6f9cf6b2023f5f679e6b0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732682"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="20478-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="20478-103">Get deviceAppManagement</span></span>

<span data-ttu-id="20478-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20478-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20478-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20478-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20478-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20478-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20478-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20478-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20478-108">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="20478-108">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20478-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20478-109">Prerequisites</span></span>

<span data-ttu-id="20478-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="20478-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="20478-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20478-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="20478-112">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="20478-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="20478-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20478-113">Permission type</span></span>|<span data-ttu-id="20478-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20478-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="20478-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20478-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="20478-116">&nbsp;&nbsp; **Aplicativos**, **livros**, **onboarding**integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="20478-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="20478-117">DeviceManagementApps. ReadWrite. All, DeviceManagementApps. ReadW. All</span><span class="sxs-lookup"><span data-stu-id="20478-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="20478-118">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="20478-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="20478-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20478-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="20478-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20478-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20478-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20478-121">Not supported.</span></span>|
|<span data-ttu-id="20478-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20478-122">Application</span></span>| |
| <span data-ttu-id="20478-123">&nbsp;&nbsp; **Aplicativos**, **livros**, **onboarding**integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="20478-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="20478-124">DeviceManagementApps. ReadWrite. All, DeviceManagementApps. ReadW. All</span><span class="sxs-lookup"><span data-stu-id="20478-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="20478-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="20478-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="20478-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20478-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20478-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20478-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20478-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20478-128">Optional query parameters</span></span>

<span data-ttu-id="20478-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20478-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20478-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20478-130">Request headers</span></span>

|<span data-ttu-id="20478-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20478-131">Header</span></span>|<span data-ttu-id="20478-132">Valor</span><span class="sxs-lookup"><span data-stu-id="20478-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20478-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="20478-133">Authorization</span></span>|<span data-ttu-id="20478-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20478-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20478-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20478-135">Accept</span></span>|<span data-ttu-id="20478-136">application/json</span><span class="sxs-lookup"><span data-stu-id="20478-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20478-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20478-137">Request body</span></span>

<span data-ttu-id="20478-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20478-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20478-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="20478-139">Response</span></span>

<span data-ttu-id="20478-140">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20478-140">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20478-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20478-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="20478-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20478-142">Request</span></span>

<span data-ttu-id="20478-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20478-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="20478-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20478-144">Response</span></span>

<span data-ttu-id="20478-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20478-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```











