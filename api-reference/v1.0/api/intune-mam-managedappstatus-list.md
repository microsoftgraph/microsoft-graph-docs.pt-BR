---
title: Listar managedAppStatuses
description: Listar propriedades e relações dos objetos managedAppStatus.
ms.openlocfilehash: c31c745b420acf8fb7ae8397830dc9125a83d343
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005574"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="af7d0-103">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="af7d0-103">List managedAppStatuses</span></span>

> <span data-ttu-id="af7d0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af7d0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af7d0-105">Listar propriedades e relações dos objetos [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="af7d0-105">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af7d0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af7d0-106">Prerequisites</span></span>
<span data-ttu-id="af7d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af7d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af7d0-109">Permission type</span></span>|<span data-ttu-id="af7d0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af7d0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af7d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af7d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af7d0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="af7d0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="af7d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af7d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af7d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af7d0-114">Not supported.</span></span>|
|<span data-ttu-id="af7d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af7d0-115">Application</span></span>|<span data-ttu-id="af7d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af7d0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af7d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af7d0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="af7d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af7d0-118">Request headers</span></span>
|<span data-ttu-id="af7d0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af7d0-119">Header</span></span>|<span data-ttu-id="af7d0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="af7d0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af7d0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="af7d0-121">Authorization</span></span>|<span data-ttu-id="af7d0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af7d0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af7d0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="af7d0-123">Accept</span></span>|<span data-ttu-id="af7d0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="af7d0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af7d0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af7d0-125">Request body</span></span>
<span data-ttu-id="af7d0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af7d0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af7d0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="af7d0-127">Response</span></span>
<span data-ttu-id="af7d0-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppStatus](../resources/intune-mam-managedappstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af7d0-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7d0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af7d0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="af7d0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af7d0-130">Request</span></span>
<span data-ttu-id="af7d0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af7d0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="af7d0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="af7d0-132">Response</span></span>
<span data-ttu-id="af7d0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af7d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



