---
title: Excluir mobileAppInstallStatus
description: Exclui um mobileAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 664a65bff49e467adbe3b5cd23b39acd3d0e9e35
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405384"
---
# <a name="delete-mobileappinstallstatus"></a><span data-ttu-id="e46c7-103">Excluir mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e46c7-103">Delete mobileAppInstallStatus</span></span>

> <span data-ttu-id="e46c7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e46c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e46c7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e46c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e46c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e46c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e46c7-107">Exclui um [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e46c7-107">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e46c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e46c7-108">Prerequisites</span></span>
<span data-ttu-id="e46c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e46c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e46c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e46c7-111">Permission type</span></span>|<span data-ttu-id="e46c7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e46c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e46c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e46c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e46c7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e46c7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e46c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e46c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e46c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e46c7-116">Not supported.</span></span>|
|<span data-ttu-id="e46c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e46c7-117">Application</span></span>|<span data-ttu-id="e46c7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e46c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e46c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e46c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e46c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e46c7-120">Request headers</span></span>
|<span data-ttu-id="e46c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e46c7-121">Header</span></span>|<span data-ttu-id="e46c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e46c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e46c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e46c7-123">Authorization</span></span>|<span data-ttu-id="e46c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e46c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e46c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e46c7-125">Accept</span></span>|<span data-ttu-id="e46c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e46c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e46c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e46c7-127">Request body</span></span>
<span data-ttu-id="e46c7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e46c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e46c7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e46c7-129">Response</span></span>
<span data-ttu-id="e46c7-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e46c7-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e46c7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e46c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e46c7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e46c7-132">Request</span></span>
<span data-ttu-id="e46c7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e46c7-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="e46c7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e46c7-134">Response</span></span>
<span data-ttu-id="e46c7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e46c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




