---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48a71e0b867bb26671b19eac4fc725330c2c42fe
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194604"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="9aef6-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="9aef6-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="9aef6-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9aef6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9aef6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9aef6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9aef6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9aef6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aef6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9aef6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9aef6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9aef6-108">Prerequisites</span></span>
<span data-ttu-id="9aef6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aef6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aef6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9aef6-111">Permission type</span></span>|<span data-ttu-id="9aef6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9aef6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9aef6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9aef6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9aef6-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="9aef6-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9aef6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aef6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9aef6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9aef6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9aef6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9aef6-117">Not supported.</span></span>|
|<span data-ttu-id="9aef6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9aef6-118">Application</span></span>||
| <span data-ttu-id="9aef6-119">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="9aef6-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9aef6-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aef6-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="9aef6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9aef6-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="9aef6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9aef6-122">Request headers</span></span>
|<span data-ttu-id="9aef6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9aef6-123">Header</span></span>|<span data-ttu-id="9aef6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="9aef6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9aef6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9aef6-125">Authorization</span></span>|<span data-ttu-id="9aef6-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9aef6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9aef6-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9aef6-127">Accept</span></span>|<span data-ttu-id="9aef6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9aef6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aef6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9aef6-129">Request body</span></span>
<span data-ttu-id="9aef6-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9aef6-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9aef6-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9aef6-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9aef6-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aef6-132">Property</span></span>|<span data-ttu-id="9aef6-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aef6-133">Type</span></span>|<span data-ttu-id="9aef6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aef6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aef6-135">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="9aef6-135">notificationTitle</span></span>|<span data-ttu-id="9aef6-136">String</span><span class="sxs-lookup"><span data-stu-id="9aef6-136">String</span></span>|<span data-ttu-id="9aef6-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9aef6-137">Not yet documented</span></span>|
|<span data-ttu-id="9aef6-138">notificationBody</span><span class="sxs-lookup"><span data-stu-id="9aef6-138">notificationBody</span></span>|<span data-ttu-id="9aef6-139">String</span><span class="sxs-lookup"><span data-stu-id="9aef6-139">String</span></span>|<span data-ttu-id="9aef6-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9aef6-140">Not yet documented</span></span>|
|<span data-ttu-id="9aef6-141">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="9aef6-141">groupsToNotify</span></span>|<span data-ttu-id="9aef6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9aef6-142">String collection</span></span>|<span data-ttu-id="9aef6-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9aef6-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9aef6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9aef6-144">Response</span></span>
<span data-ttu-id="9aef6-145">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9aef6-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9aef6-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9aef6-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="9aef6-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9aef6-147">Request</span></span>
<span data-ttu-id="9aef6-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9aef6-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9aef6-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9aef6-149">Response</span></span>
<span data-ttu-id="9aef6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9aef6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










