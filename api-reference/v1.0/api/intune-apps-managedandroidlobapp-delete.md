---
title: Excluir managedAndroidLobApp
description: Exclui managedAndroidLobApp.
ms.openlocfilehash: 2aaf56ca59834d3814fc7533669cd2ce8617a2a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006975"
---
# <a name="delete-managedandroidlobapp"></a><span data-ttu-id="fe31f-103">Excluir managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="fe31f-103">Delete managedAndroidLobApp</span></span>

> <span data-ttu-id="fe31f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fe31f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe31f-105">Exclui [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe31f-105">Deletes a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe31f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe31f-106">Prerequisites</span></span>
<span data-ttu-id="fe31f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe31f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe31f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe31f-109">Permission type</span></span>|<span data-ttu-id="fe31f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe31f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe31f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe31f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe31f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe31f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe31f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe31f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe31f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe31f-114">Not supported.</span></span>|
|<span data-ttu-id="fe31f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe31f-115">Application</span></span>|<span data-ttu-id="fe31f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe31f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe31f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe31f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="fe31f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe31f-118">Request headers</span></span>
|<span data-ttu-id="fe31f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe31f-119">Header</span></span>|<span data-ttu-id="fe31f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fe31f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe31f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe31f-121">Authorization</span></span>|<span data-ttu-id="fe31f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe31f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe31f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fe31f-123">Accept</span></span>|<span data-ttu-id="fe31f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fe31f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe31f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe31f-125">Request body</span></span>
<span data-ttu-id="fe31f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe31f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe31f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe31f-127">Response</span></span>
<span data-ttu-id="fe31f-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fe31f-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe31f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe31f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe31f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe31f-130">Request</span></span>
<span data-ttu-id="fe31f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe31f-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="fe31f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe31f-132">Response</span></span>
<span data-ttu-id="fe31f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe31f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



