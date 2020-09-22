---
title: Get managedAppStatusRaw
description: Ler propriedades e relações do objeto managedAppStatusRaw.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 999308acd475cad8073b7dbac6082570e7632955
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044071"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="3aad0-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3aad0-103">Get managedAppStatusRaw</span></span>

<span data-ttu-id="3aad0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aad0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3aad0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3aad0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3aad0-106">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="3aad0-106">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3aad0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3aad0-107">Prerequisites</span></span>
<span data-ttu-id="3aad0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aad0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aad0-110">Permission type</span></span>|<span data-ttu-id="3aad0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3aad0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aad0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aad0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3aad0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aad0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3aad0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aad0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aad0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aad0-115">Not supported.</span></span>|
|<span data-ttu-id="3aad0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aad0-116">Application</span></span>|<span data-ttu-id="3aad0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aad0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aad0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aad0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3aad0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3aad0-119">Optional query parameters</span></span>
<span data-ttu-id="3aad0-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3aad0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aad0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aad0-121">Request headers</span></span>
|<span data-ttu-id="3aad0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3aad0-122">Header</span></span>|<span data-ttu-id="3aad0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3aad0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aad0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aad0-124">Authorization</span></span>|<span data-ttu-id="3aad0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aad0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aad0-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3aad0-126">Accept</span></span>|<span data-ttu-id="3aad0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3aad0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aad0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aad0-128">Request body</span></span>
<span data-ttu-id="3aad0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3aad0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aad0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aad0-130">Response</span></span>
<span data-ttu-id="3aad0-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aad0-131">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aad0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aad0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3aad0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aad0-133">Request</span></span>
<span data-ttu-id="3aad0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aad0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="3aad0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aad0-135">Response</span></span>
<span data-ttu-id="3aad0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aad0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









