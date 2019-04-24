---
title: ação revokeAllLicenses
description: Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 708065bb16fa5435aada4e888d95f489df4924a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495572"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="56342-103">ação revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="56342-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="56342-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56342-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56342-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56342-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56342-106">Revoga todas as licenças VPP do iOS atribuídas para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="56342-106">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56342-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56342-107">Prerequisites</span></span>
<span data-ttu-id="56342-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56342-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56342-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56342-110">Permission type</span></span>|<span data-ttu-id="56342-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56342-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56342-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56342-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56342-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56342-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56342-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56342-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56342-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56342-115">Not supported.</span></span>|
|<span data-ttu-id="56342-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56342-116">Application</span></span>|<span data-ttu-id="56342-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56342-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56342-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56342-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="56342-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56342-119">Request headers</span></span>
|<span data-ttu-id="56342-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56342-120">Header</span></span>|<span data-ttu-id="56342-121">Valor</span><span class="sxs-lookup"><span data-stu-id="56342-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56342-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56342-122">Authorization</span></span>|<span data-ttu-id="56342-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56342-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56342-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56342-124">Accept</span></span>|<span data-ttu-id="56342-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56342-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56342-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56342-126">Request body</span></span>
<span data-ttu-id="56342-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="56342-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56342-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="56342-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56342-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56342-129">Property</span></span>|<span data-ttu-id="56342-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="56342-130">Type</span></span>|<span data-ttu-id="56342-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="56342-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56342-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="56342-132">notifyManagedDevices</span></span>|<span data-ttu-id="56342-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="56342-133">Boolean</span></span>|<span data-ttu-id="56342-134">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="56342-134">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="56342-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="56342-135">Response</span></span>
<span data-ttu-id="56342-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56342-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56342-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56342-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="56342-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56342-138">Request</span></span>
<span data-ttu-id="56342-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56342-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="56342-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="56342-140">Response</span></span>
<span data-ttu-id="56342-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56342-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





