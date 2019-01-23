---
title: Get managedAppStatusRaw
description: Ler propriedades e relações do objeto managedAppStatusRaw.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30bae06ff10b369a83f11ac50f169449e5cc0cc8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399917"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="9f13e-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9f13e-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="9f13e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f13e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f13e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f13e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f13e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9f13e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f13e-107">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9f13e-107">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f13e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f13e-108">Prerequisites</span></span>
<span data-ttu-id="9f13e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f13e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f13e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f13e-111">Permission type</span></span>|<span data-ttu-id="9f13e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f13e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f13e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f13e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f13e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f13e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9f13e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f13e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f13e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f13e-116">Not supported.</span></span>|
|<span data-ttu-id="9f13e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f13e-117">Application</span></span>|<span data-ttu-id="9f13e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f13e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f13e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f13e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f13e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f13e-120">Optional query parameters</span></span>
<span data-ttu-id="9f13e-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13e-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f13e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13e-122">Request headers</span></span>
|<span data-ttu-id="9f13e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f13e-123">Header</span></span>|<span data-ttu-id="9f13e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="9f13e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f13e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f13e-125">Authorization</span></span>|<span data-ttu-id="9f13e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f13e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f13e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f13e-127">Accept</span></span>|<span data-ttu-id="9f13e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f13e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f13e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13e-129">Request body</span></span>
<span data-ttu-id="9f13e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f13e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f13e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13e-131">Response</span></span>
<span data-ttu-id="9f13e-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13e-132">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f13e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f13e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f13e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13e-134">Request</span></span>
<span data-ttu-id="9f13e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f13e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="9f13e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13e-136">Response</span></span>
<span data-ttu-id="9f13e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f13e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```




