---
title: Excluir windowsPhoneXAP
description: Exclui windowsPhoneXAP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19b27fcb09c76d20952ae8de5bd6f8d810ff6518
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781229"
---
# <a name="delete-windowsphonexap"></a><span data-ttu-id="114ac-103">Excluir windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="114ac-103">Delete windowsPhoneXAP</span></span>

> <span data-ttu-id="114ac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="114ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="114ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="114ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="114ac-106">Exclui [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="114ac-106">Deletes a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="114ac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="114ac-107">Prerequisites</span></span>
<span data-ttu-id="114ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="114ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="114ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="114ac-110">Permission type</span></span>|<span data-ttu-id="114ac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="114ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="114ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="114ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="114ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="114ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="114ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="114ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="114ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="114ac-115">Not supported.</span></span>|
|<span data-ttu-id="114ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="114ac-116">Application</span></span>|<span data-ttu-id="114ac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="114ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="114ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="114ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="114ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="114ac-119">Request headers</span></span>
|<span data-ttu-id="114ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="114ac-120">Header</span></span>|<span data-ttu-id="114ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="114ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="114ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="114ac-122">Authorization</span></span>|<span data-ttu-id="114ac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="114ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="114ac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="114ac-124">Accept</span></span>|<span data-ttu-id="114ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="114ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="114ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="114ac-126">Request body</span></span>
<span data-ttu-id="114ac-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="114ac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="114ac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="114ac-128">Response</span></span>
<span data-ttu-id="114ac-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="114ac-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="114ac-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="114ac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="114ac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="114ac-131">Request</span></span>
<span data-ttu-id="114ac-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="114ac-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="114ac-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="114ac-133">Response</span></span>
<span data-ttu-id="114ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="114ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





