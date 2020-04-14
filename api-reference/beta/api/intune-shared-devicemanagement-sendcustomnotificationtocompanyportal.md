---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf850c6bb6866c0f71d6da869e63b5d73f6288d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390056"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="fb2b0-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="fb2b0-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="fb2b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb2b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb2b0-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb2b0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb2b0-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb2b0-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb2b0-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb2b0-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb2b0-109">Prerequisites</span></span>
<span data-ttu-id="fb2b0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb2b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb2b0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb2b0-112">Permission type</span></span>|<span data-ttu-id="fb2b0-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb2b0-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb2b0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb2b0-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fb2b0-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fb2b0-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fb2b0-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb2b0-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb2b0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb2b0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb2b0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-118">Not supported.</span></span>|
|<span data-ttu-id="fb2b0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb2b0-119">Application</span></span>||
| <span data-ttu-id="fb2b0-120">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fb2b0-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fb2b0-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb2b0-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="fb2b0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb2b0-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="fb2b0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb2b0-123">Request headers</span></span>
|<span data-ttu-id="fb2b0-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb2b0-124">Header</span></span>|<span data-ttu-id="fb2b0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="fb2b0-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb2b0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb2b0-126">Authorization</span></span>|<span data-ttu-id="fb2b0-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb2b0-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb2b0-128">Accept</span></span>|<span data-ttu-id="fb2b0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fb2b0-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb2b0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb2b0-130">Request body</span></span>
<span data-ttu-id="fb2b0-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fb2b0-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fb2b0-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb2b0-133">Property</span></span>|<span data-ttu-id="fb2b0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb2b0-134">Type</span></span>|<span data-ttu-id="fb2b0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb2b0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb2b0-136">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="fb2b0-136">notificationTitle</span></span>|<span data-ttu-id="fb2b0-137">String</span><span class="sxs-lookup"><span data-stu-id="fb2b0-137">String</span></span>|<span data-ttu-id="fb2b0-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb2b0-138">Not yet documented</span></span>|
|<span data-ttu-id="fb2b0-139">notificationBody</span><span class="sxs-lookup"><span data-stu-id="fb2b0-139">notificationBody</span></span>|<span data-ttu-id="fb2b0-140">String</span><span class="sxs-lookup"><span data-stu-id="fb2b0-140">String</span></span>|<span data-ttu-id="fb2b0-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb2b0-141">Not yet documented</span></span>|
|<span data-ttu-id="fb2b0-142">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="fb2b0-142">groupsToNotify</span></span>|<span data-ttu-id="fb2b0-143">String collection</span><span class="sxs-lookup"><span data-stu-id="fb2b0-143">String collection</span></span>|<span data-ttu-id="fb2b0-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb2b0-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fb2b0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb2b0-145">Response</span></span>
<span data-ttu-id="fb2b0-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb2b0-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb2b0-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb2b0-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb2b0-148">Request</span></span>
<span data-ttu-id="fb2b0-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb2b0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb2b0-150">Response</span></span>
<span data-ttu-id="fb2b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb2b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












