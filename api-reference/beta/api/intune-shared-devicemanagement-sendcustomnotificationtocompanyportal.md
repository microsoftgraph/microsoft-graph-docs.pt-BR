---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b6663c86676982149e42945a8db82c4a6a84aa0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210137"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="bf0da-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="bf0da-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="bf0da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf0da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf0da-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf0da-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf0da-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf0da-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf0da-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf0da-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf0da-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bf0da-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf0da-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bf0da-109">Prerequisites</span></span>
<span data-ttu-id="bf0da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf0da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0da-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf0da-112">Permission type</span></span>|<span data-ttu-id="bf0da-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bf0da-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf0da-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf0da-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bf0da-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="bf0da-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bf0da-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf0da-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bf0da-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf0da-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf0da-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf0da-118">Not supported.</span></span>|
|<span data-ttu-id="bf0da-119">Application</span><span class="sxs-lookup"><span data-stu-id="bf0da-119">Application</span></span>||
| <span data-ttu-id="bf0da-120">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="bf0da-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bf0da-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf0da-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="bf0da-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf0da-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="bf0da-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf0da-123">Request headers</span></span>
|<span data-ttu-id="bf0da-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf0da-124">Header</span></span>|<span data-ttu-id="bf0da-125">Valor</span><span class="sxs-lookup"><span data-stu-id="bf0da-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf0da-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf0da-126">Authorization</span></span>|<span data-ttu-id="bf0da-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf0da-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf0da-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bf0da-128">Accept</span></span>|<span data-ttu-id="bf0da-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bf0da-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf0da-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf0da-130">Request body</span></span>
<span data-ttu-id="bf0da-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bf0da-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bf0da-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="bf0da-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bf0da-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf0da-133">Property</span></span>|<span data-ttu-id="bf0da-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf0da-134">Type</span></span>|<span data-ttu-id="bf0da-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf0da-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf0da-136">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="bf0da-136">notificationTitle</span></span>|<span data-ttu-id="bf0da-137">String</span><span class="sxs-lookup"><span data-stu-id="bf0da-137">String</span></span>|<span data-ttu-id="bf0da-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bf0da-138">Not yet documented</span></span>|
|<span data-ttu-id="bf0da-139">notificationBody</span><span class="sxs-lookup"><span data-stu-id="bf0da-139">notificationBody</span></span>|<span data-ttu-id="bf0da-140">String</span><span class="sxs-lookup"><span data-stu-id="bf0da-140">String</span></span>|<span data-ttu-id="bf0da-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bf0da-141">Not yet documented</span></span>|
|<span data-ttu-id="bf0da-142">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="bf0da-142">groupsToNotify</span></span>|<span data-ttu-id="bf0da-143">String collection</span><span class="sxs-lookup"><span data-stu-id="bf0da-143">String collection</span></span>|<span data-ttu-id="bf0da-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bf0da-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bf0da-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf0da-145">Response</span></span>
<span data-ttu-id="bf0da-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf0da-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf0da-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf0da-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf0da-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf0da-148">Request</span></span>
<span data-ttu-id="bf0da-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf0da-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bf0da-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf0da-150">Response</span></span>
<span data-ttu-id="bf0da-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf0da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













