---
title: Excluir iosVppApp
description: Exclui iosVppApp.
ms.openlocfilehash: 609c283255011f1f24c683f3de281d628f036737
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003839"
---
# <a name="delete-iosvppapp"></a><span data-ttu-id="89836-103">Excluir iosVppApp</span><span class="sxs-lookup"><span data-stu-id="89836-103">Delete iosVppApp</span></span>

> <span data-ttu-id="89836-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="89836-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89836-105">Exclui [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="89836-105">Deletes a [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89836-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89836-106">Prerequisites</span></span>
<span data-ttu-id="89836-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89836-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89836-109">Permission type</span></span>|<span data-ttu-id="89836-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89836-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89836-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89836-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89836-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89836-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89836-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89836-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89836-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89836-114">Not supported.</span></span>|
|<span data-ttu-id="89836-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89836-115">Application</span></span>|<span data-ttu-id="89836-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89836-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89836-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89836-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="89836-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89836-118">Request headers</span></span>
|<span data-ttu-id="89836-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89836-119">Header</span></span>|<span data-ttu-id="89836-120">Valor</span><span class="sxs-lookup"><span data-stu-id="89836-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89836-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="89836-121">Authorization</span></span>|<span data-ttu-id="89836-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89836-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89836-123">Accept</span><span class="sxs-lookup"><span data-stu-id="89836-123">Accept</span></span>|<span data-ttu-id="89836-124">application/json</span><span class="sxs-lookup"><span data-stu-id="89836-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89836-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89836-125">Request body</span></span>
<span data-ttu-id="89836-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89836-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89836-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="89836-127">Response</span></span>
<span data-ttu-id="89836-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="89836-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="89836-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89836-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="89836-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89836-130">Request</span></span>
<span data-ttu-id="89836-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89836-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="89836-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="89836-132">Response</span></span>
<span data-ttu-id="89836-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89836-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



