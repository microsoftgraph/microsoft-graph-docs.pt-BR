---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efdadb8e5e87eecf0d70102d261a9f4d87a6468a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347553"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="68cf6-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="68cf6-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="68cf6-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="68cf6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68cf6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="68cf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68cf6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68cf6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68cf6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68cf6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68cf6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68cf6-108">Prerequisites</span></span>
<span data-ttu-id="68cf6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68cf6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68cf6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68cf6-111">Permission type</span></span>|<span data-ttu-id="68cf6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68cf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68cf6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68cf6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="68cf6-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="68cf6-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="68cf6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cf6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="68cf6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68cf6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68cf6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68cf6-117">Not supported.</span></span>|
|<span data-ttu-id="68cf6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68cf6-118">Application</span></span>|<span data-ttu-id="68cf6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68cf6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68cf6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68cf6-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="68cf6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68cf6-121">Request headers</span></span>
|<span data-ttu-id="68cf6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68cf6-122">Header</span></span>|<span data-ttu-id="68cf6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="68cf6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68cf6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="68cf6-124">Authorization</span></span>|<span data-ttu-id="68cf6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68cf6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68cf6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68cf6-126">Accept</span></span>|<span data-ttu-id="68cf6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="68cf6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68cf6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68cf6-128">Request body</span></span>
<span data-ttu-id="68cf6-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="68cf6-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="68cf6-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="68cf6-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="68cf6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68cf6-131">Property</span></span>|<span data-ttu-id="68cf6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="68cf6-132">Type</span></span>|<span data-ttu-id="68cf6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="68cf6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68cf6-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="68cf6-134">notificationTitle</span></span>|<span data-ttu-id="68cf6-135">String</span><span class="sxs-lookup"><span data-stu-id="68cf6-135">String</span></span>|<span data-ttu-id="68cf6-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68cf6-136">Not yet documented</span></span>|
|<span data-ttu-id="68cf6-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="68cf6-137">notificationBody</span></span>|<span data-ttu-id="68cf6-138">String</span><span class="sxs-lookup"><span data-stu-id="68cf6-138">String</span></span>|<span data-ttu-id="68cf6-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68cf6-139">Not yet documented</span></span>|
|<span data-ttu-id="68cf6-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="68cf6-140">groupsToNotify</span></span>|<span data-ttu-id="68cf6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="68cf6-141">String collection</span></span>|<span data-ttu-id="68cf6-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68cf6-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="68cf6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="68cf6-143">Response</span></span>
<span data-ttu-id="68cf6-144">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68cf6-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68cf6-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68cf6-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="68cf6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68cf6-146">Request</span></span>
<span data-ttu-id="68cf6-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68cf6-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68cf6-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="68cf6-148">Response</span></span>
<span data-ttu-id="68cf6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68cf6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









