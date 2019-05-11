---
title: ação revokeAllLicenses
description: Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 286c9966b143ed65609cbbfd13d742c4594e6465
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937390"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="39eea-103">ação revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="39eea-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="39eea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39eea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39eea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39eea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39eea-106">Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39eea-106">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39eea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39eea-107">Prerequisites</span></span>
<span data-ttu-id="39eea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39eea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39eea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39eea-110">Permission type</span></span>|<span data-ttu-id="39eea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39eea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39eea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39eea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39eea-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39eea-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39eea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39eea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39eea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39eea-115">Not supported.</span></span>|
|<span data-ttu-id="39eea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39eea-116">Application</span></span>|<span data-ttu-id="39eea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39eea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39eea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39eea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="39eea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39eea-119">Request headers</span></span>
|<span data-ttu-id="39eea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39eea-120">Header</span></span>|<span data-ttu-id="39eea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="39eea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39eea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="39eea-122">Authorization</span></span>|<span data-ttu-id="39eea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39eea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39eea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39eea-124">Accept</span></span>|<span data-ttu-id="39eea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39eea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39eea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39eea-126">Request body</span></span>
<span data-ttu-id="39eea-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="39eea-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="39eea-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="39eea-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="39eea-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39eea-129">Property</span></span>|<span data-ttu-id="39eea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="39eea-130">Type</span></span>|<span data-ttu-id="39eea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="39eea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39eea-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="39eea-132">notifyManagedDevices</span></span>|<span data-ttu-id="39eea-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="39eea-133">Boolean</span></span>|<span data-ttu-id="39eea-134">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="39eea-134">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="39eea-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="39eea-135">Response</span></span>
<span data-ttu-id="39eea-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39eea-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39eea-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39eea-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="39eea-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39eea-138">Request</span></span>
<span data-ttu-id="39eea-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39eea-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="39eea-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="39eea-140">Response</span></span>
<span data-ttu-id="39eea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39eea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




