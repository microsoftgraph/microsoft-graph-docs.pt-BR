---
title: Listar managedAppStatuses
description: Listar propriedades e relações dos objetos managedAppStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4f23d0bababd6736c906c15d22c374fdd6885a3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513074"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="98a73-103">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="98a73-103">List managedAppStatuses</span></span>

<span data-ttu-id="98a73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98a73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98a73-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98a73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98a73-106">Listar propriedades e relações dos objetos [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="98a73-106">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98a73-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98a73-107">Prerequisites</span></span>
<span data-ttu-id="98a73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98a73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98a73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98a73-110">Permission type</span></span>|<span data-ttu-id="98a73-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98a73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98a73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98a73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98a73-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="98a73-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="98a73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98a73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98a73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98a73-115">Not supported.</span></span>|
|<span data-ttu-id="98a73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98a73-116">Application</span></span>|<span data-ttu-id="98a73-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98a73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98a73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98a73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="98a73-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98a73-119">Request headers</span></span>
|<span data-ttu-id="98a73-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98a73-120">Header</span></span>|<span data-ttu-id="98a73-121">Valor</span><span class="sxs-lookup"><span data-stu-id="98a73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98a73-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98a73-122">Authorization</span></span>|<span data-ttu-id="98a73-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98a73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98a73-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98a73-124">Accept</span></span>|<span data-ttu-id="98a73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98a73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98a73-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98a73-126">Request body</span></span>
<span data-ttu-id="98a73-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98a73-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98a73-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="98a73-128">Response</span></span>
<span data-ttu-id="98a73-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppStatus](../resources/intune-mam-managedappstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98a73-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98a73-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98a73-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="98a73-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98a73-131">Request</span></span>
<span data-ttu-id="98a73-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98a73-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="98a73-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="98a73-133">Response</span></span>
<span data-ttu-id="98a73-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98a73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatus",
      "displayName": "Display Name value",
      "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
      "version": "Version value"
    }
  ]
}
```




