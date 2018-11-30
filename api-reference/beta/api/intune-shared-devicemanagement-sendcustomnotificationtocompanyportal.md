---
title: ação de sendCustomNotificationToCompanyPortal
description: Ainda não documentado
ms.openlocfilehash: bf19f87c385568a38407fff0df144c6df165fbc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035716"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="8309a-103">ação de sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="8309a-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="8309a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8309a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8309a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8309a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8309a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8309a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8309a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8309a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8309a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8309a-108">Prerequisites</span></span>
<span data-ttu-id="8309a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8309a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8309a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8309a-111">Permission type</span></span>|<span data-ttu-id="8309a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8309a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8309a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8309a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8309a-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8309a-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8309a-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8309a-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8309a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8309a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8309a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8309a-117">Not supported.</span></span>|
|<span data-ttu-id="8309a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8309a-118">Application</span></span>|<span data-ttu-id="8309a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8309a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8309a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8309a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="8309a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8309a-121">Request headers</span></span>
|<span data-ttu-id="8309a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8309a-122">Header</span></span>|<span data-ttu-id="8309a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8309a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8309a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8309a-124">Authorization</span></span>|<span data-ttu-id="8309a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8309a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8309a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8309a-126">Accept</span></span>|<span data-ttu-id="8309a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8309a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8309a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8309a-128">Request body</span></span>
<span data-ttu-id="8309a-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8309a-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8309a-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8309a-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8309a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8309a-131">Property</span></span>|<span data-ttu-id="8309a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8309a-132">Type</span></span>|<span data-ttu-id="8309a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8309a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8309a-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="8309a-134">notificationTitle</span></span>|<span data-ttu-id="8309a-135">String</span><span class="sxs-lookup"><span data-stu-id="8309a-135">String</span></span>|<span data-ttu-id="8309a-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8309a-136">Not yet documented</span></span>|
|<span data-ttu-id="8309a-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="8309a-137">notificationBody</span></span>|<span data-ttu-id="8309a-138">String</span><span class="sxs-lookup"><span data-stu-id="8309a-138">String</span></span>|<span data-ttu-id="8309a-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8309a-139">Not yet documented</span></span>|
|<span data-ttu-id="8309a-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="8309a-140">groupsToNotify</span></span>|<span data-ttu-id="8309a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8309a-141">String collection</span></span>|<span data-ttu-id="8309a-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8309a-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8309a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8309a-143">Response</span></span>
<span data-ttu-id="8309a-144">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8309a-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8309a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8309a-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="8309a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8309a-146">Request</span></span>
<span data-ttu-id="8309a-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8309a-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 164

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "groupsToNotify": [
    "Groups To Notify value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8309a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8309a-148">Response</span></span>
<span data-ttu-id="8309a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8309a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






