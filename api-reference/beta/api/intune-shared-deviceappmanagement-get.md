---
title: Get deviceAppManagement
description: Ler propriedades e relações do objeto deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c27099cdc0e2ffbbc3e0e02cde07b9b4e34ea33c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963510"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="1689a-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1689a-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="1689a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1689a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1689a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1689a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1689a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1689a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1689a-107">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1689a-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1689a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1689a-108">Prerequisites</span></span>

<span data-ttu-id="1689a-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1689a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1689a-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1689a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="1689a-111">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1689a-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="1689a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1689a-112">Permission type</span></span>|<span data-ttu-id="1689a-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1689a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="1689a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1689a-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="1689a-115">&nbsp;&nbsp; **Aplicativos**, **livros**ou **integração**</span><span class="sxs-lookup"><span data-stu-id="1689a-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="1689a-116">DeviceManagementApps. ReadWrite. All, DeviceManagementApps. ReadW. All</span><span class="sxs-lookup"><span data-stu-id="1689a-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="1689a-117">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1689a-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1689a-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1689a-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="1689a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1689a-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1689a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1689a-120">Not supported.</span></span>|
|<span data-ttu-id="1689a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1689a-121">Application</span></span>|<span data-ttu-id="1689a-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1689a-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1689a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1689a-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1689a-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1689a-124">Optional query parameters</span></span>

<span data-ttu-id="1689a-125">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1689a-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1689a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1689a-126">Request headers</span></span>

|<span data-ttu-id="1689a-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1689a-127">Header</span></span>|<span data-ttu-id="1689a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1689a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1689a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1689a-129">Authorization</span></span>|<span data-ttu-id="1689a-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1689a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1689a-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1689a-131">Accept</span></span>|<span data-ttu-id="1689a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1689a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1689a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1689a-133">Request body</span></span>

<span data-ttu-id="1689a-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1689a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1689a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1689a-135">Response</span></span>

<span data-ttu-id="1689a-136">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1689a-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1689a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1689a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1689a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1689a-138">Request</span></span>

<span data-ttu-id="1689a-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1689a-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="1689a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1689a-140">Response</span></span>

<span data-ttu-id="1689a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1689a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



