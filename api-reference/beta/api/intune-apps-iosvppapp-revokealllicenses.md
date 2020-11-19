---
title: ação revokeAllLicenses
description: Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6eae639a694d2e23d437453c07c0c0a71f8bb4b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252393"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="6bfdd-103">ação revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="6bfdd-103">revokeAllLicenses action</span></span>

<span data-ttu-id="6bfdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bfdd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bfdd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bfdd-107">Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-107">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bfdd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bfdd-108">Prerequisites</span></span>
<span data-ttu-id="6bfdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bfdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bfdd-111">Permission type</span></span>|<span data-ttu-id="6bfdd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bfdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bfdd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bfdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bfdd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bfdd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6bfdd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bfdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bfdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-116">Not supported.</span></span>|
|<span data-ttu-id="6bfdd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bfdd-117">Application</span></span>|<span data-ttu-id="6bfdd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bfdd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bfdd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="6bfdd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfdd-120">Request headers</span></span>
|<span data-ttu-id="6bfdd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bfdd-121">Header</span></span>|<span data-ttu-id="6bfdd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6bfdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bfdd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bfdd-123">Authorization</span></span>|<span data-ttu-id="6bfdd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bfdd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bfdd-125">Accept</span></span>|<span data-ttu-id="6bfdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bfdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bfdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfdd-127">Request body</span></span>
<span data-ttu-id="6bfdd-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6bfdd-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6bfdd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bfdd-130">Property</span></span>|<span data-ttu-id="6bfdd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bfdd-131">Type</span></span>|<span data-ttu-id="6bfdd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bfdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bfdd-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="6bfdd-133">notifyManagedDevices</span></span>|<span data-ttu-id="6bfdd-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="6bfdd-134">Boolean</span></span>|<span data-ttu-id="6bfdd-135">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="6bfdd-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="6bfdd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bfdd-136">Response</span></span>
<span data-ttu-id="6bfdd-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6bfdd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bfdd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bfdd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfdd-139">Request</span></span>
<span data-ttu-id="6bfdd-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="6bfdd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bfdd-141">Response</span></span>
<span data-ttu-id="6bfdd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bfdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




