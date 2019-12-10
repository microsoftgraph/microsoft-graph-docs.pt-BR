---
title: ação revokeAllLicenses
description: Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a11be182f023377c7bc052923f2c6a85f3d81bd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39925610"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="e37bf-103">ação revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="e37bf-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="e37bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e37bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e37bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e37bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e37bf-106">Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e37bf-106">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e37bf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e37bf-107">Prerequisites</span></span>
<span data-ttu-id="e37bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e37bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e37bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e37bf-110">Permission type</span></span>|<span data-ttu-id="e37bf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e37bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e37bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e37bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e37bf-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e37bf-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e37bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e37bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e37bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e37bf-115">Not supported.</span></span>|
|<span data-ttu-id="e37bf-116">Application</span><span class="sxs-lookup"><span data-stu-id="e37bf-116">Application</span></span>|<span data-ttu-id="e37bf-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e37bf-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e37bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e37bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="e37bf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e37bf-119">Request headers</span></span>
|<span data-ttu-id="e37bf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e37bf-120">Header</span></span>|<span data-ttu-id="e37bf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e37bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e37bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e37bf-122">Authorization</span></span>|<span data-ttu-id="e37bf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e37bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e37bf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e37bf-124">Accept</span></span>|<span data-ttu-id="e37bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e37bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e37bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e37bf-126">Request body</span></span>
<span data-ttu-id="e37bf-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e37bf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e37bf-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e37bf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e37bf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e37bf-129">Property</span></span>|<span data-ttu-id="e37bf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e37bf-130">Type</span></span>|<span data-ttu-id="e37bf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e37bf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e37bf-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="e37bf-132">notifyManagedDevices</span></span>|<span data-ttu-id="e37bf-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e37bf-133">Boolean</span></span>|<span data-ttu-id="e37bf-134">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="e37bf-134">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="e37bf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e37bf-135">Response</span></span>
<span data-ttu-id="e37bf-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e37bf-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e37bf-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e37bf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e37bf-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e37bf-138">Request</span></span>
<span data-ttu-id="e37bf-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e37bf-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="e37bf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e37bf-140">Response</span></span>
<span data-ttu-id="e37bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e37bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





