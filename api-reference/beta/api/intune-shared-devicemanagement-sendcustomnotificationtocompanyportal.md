---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed98614436bf5cd6c9adea9b5c7d1059c34ec141
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801037"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="89faf-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="89faf-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="89faf-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="89faf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="89faf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89faf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89faf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89faf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89faf-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89faf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89faf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89faf-108">Prerequisites</span></span>
<span data-ttu-id="89faf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89faf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89faf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89faf-111">Permission type</span></span>|<span data-ttu-id="89faf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89faf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89faf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89faf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="89faf-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="89faf-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="89faf-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89faf-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="89faf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89faf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89faf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89faf-117">Not supported.</span></span>|
|<span data-ttu-id="89faf-118">Application</span><span class="sxs-lookup"><span data-stu-id="89faf-118">Application</span></span>||
| <span data-ttu-id="89faf-119">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="89faf-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="89faf-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89faf-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="89faf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89faf-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="89faf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89faf-122">Request headers</span></span>
|<span data-ttu-id="89faf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89faf-123">Header</span></span>|<span data-ttu-id="89faf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="89faf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89faf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="89faf-125">Authorization</span></span>|<span data-ttu-id="89faf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89faf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89faf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89faf-127">Accept</span></span>|<span data-ttu-id="89faf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="89faf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89faf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89faf-129">Request body</span></span>
<span data-ttu-id="89faf-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="89faf-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="89faf-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="89faf-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="89faf-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89faf-132">Property</span></span>|<span data-ttu-id="89faf-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="89faf-133">Type</span></span>|<span data-ttu-id="89faf-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="89faf-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89faf-135">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="89faf-135">notificationTitle</span></span>|<span data-ttu-id="89faf-136">String</span><span class="sxs-lookup"><span data-stu-id="89faf-136">String</span></span>|<span data-ttu-id="89faf-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89faf-137">Not yet documented</span></span>|
|<span data-ttu-id="89faf-138">notificationBody</span><span class="sxs-lookup"><span data-stu-id="89faf-138">notificationBody</span></span>|<span data-ttu-id="89faf-139">String</span><span class="sxs-lookup"><span data-stu-id="89faf-139">String</span></span>|<span data-ttu-id="89faf-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89faf-140">Not yet documented</span></span>|
|<span data-ttu-id="89faf-141">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="89faf-141">groupsToNotify</span></span>|<span data-ttu-id="89faf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="89faf-142">String collection</span></span>|<span data-ttu-id="89faf-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89faf-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89faf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="89faf-144">Response</span></span>
<span data-ttu-id="89faf-145">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="89faf-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="89faf-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89faf-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="89faf-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89faf-147">Request</span></span>
<span data-ttu-id="89faf-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89faf-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89faf-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="89faf-149">Response</span></span>
<span data-ttu-id="89faf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89faf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













