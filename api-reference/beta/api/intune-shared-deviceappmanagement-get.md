---
title: Get deviceAppManagement
description: Ler propriedades e relações do objeto deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f4ce05f838b88bbe2f930557b4e2384347be4ac
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086260"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="d79c1-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="d79c1-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="d79c1-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d79c1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d79c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d79c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d79c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d79c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d79c1-107">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d79c1-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d79c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d79c1-108">Prerequisites</span></span>

<span data-ttu-id="d79c1-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d79c1-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d79c1-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d79c1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="d79c1-111">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d79c1-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="d79c1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d79c1-112">Permission type</span></span>|<span data-ttu-id="d79c1-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d79c1-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="d79c1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d79c1-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="d79c1-115">&nbsp;&nbsp; **Aplicativos**, **livros**, \*\*\*\* integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="d79c1-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="d79c1-116">DeviceManagementApps. ReadWrite. All, DeviceManagementApps. ReadW. All</span><span class="sxs-lookup"><span data-stu-id="d79c1-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="d79c1-117">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d79c1-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d79c1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d79c1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="d79c1-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d79c1-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d79c1-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d79c1-120">Not supported.</span></span>|
|<span data-ttu-id="d79c1-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d79c1-121">Application</span></span>| |
| <span data-ttu-id="d79c1-122">&nbsp;&nbsp; **Aplicativos**, **livros**, \*\*\*\* integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="d79c1-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="d79c1-123">DeviceManagementApps. ReadWrite. All, DeviceManagementApps. ReadW. All</span><span class="sxs-lookup"><span data-stu-id="d79c1-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="d79c1-124">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d79c1-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d79c1-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d79c1-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d79c1-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d79c1-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d79c1-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d79c1-127">Optional query parameters</span></span>

<span data-ttu-id="d79c1-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d79c1-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d79c1-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d79c1-129">Request headers</span></span>

|<span data-ttu-id="d79c1-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d79c1-130">Header</span></span>|<span data-ttu-id="d79c1-131">Valor</span><span class="sxs-lookup"><span data-stu-id="d79c1-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d79c1-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d79c1-132">Authorization</span></span>|<span data-ttu-id="d79c1-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d79c1-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d79c1-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d79c1-134">Accept</span></span>|<span data-ttu-id="d79c1-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d79c1-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d79c1-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d79c1-136">Request body</span></span>

<span data-ttu-id="d79c1-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d79c1-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d79c1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d79c1-138">Response</span></span>

<span data-ttu-id="d79c1-139">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d79c1-139">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d79c1-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d79c1-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d79c1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d79c1-141">Request</span></span>

<span data-ttu-id="d79c1-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d79c1-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="d79c1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d79c1-143">Response</span></span>

<span data-ttu-id="d79c1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d79c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












