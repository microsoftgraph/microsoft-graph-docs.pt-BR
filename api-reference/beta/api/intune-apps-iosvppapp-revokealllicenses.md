---
title: ação de revokeAllLicenses
description: IOS REVOKE todos atribuído VPP licencia para determinados aplicativos.
author: tfitzmac
ms.openlocfilehash: 970882bd4195ef0b478790d21f6addc937f9fd50
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309230"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="4ec81-103">ação de revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="4ec81-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="4ec81-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ec81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ec81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ec81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ec81-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ec81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ec81-107">IOS REVOKE todos atribuído VPP licencia para determinados aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4ec81-107">Revoke all assigned iOS VPP licenses for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ec81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ec81-108">Prerequisites</span></span>
<span data-ttu-id="4ec81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ec81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ec81-111">Permission type</span></span>|<span data-ttu-id="4ec81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ec81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ec81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ec81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ec81-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec81-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4ec81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ec81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ec81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec81-116">Not supported.</span></span>|
|<span data-ttu-id="4ec81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ec81-117">Application</span></span>|<span data-ttu-id="4ec81-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ec81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="4ec81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec81-120">Request headers</span></span>
|<span data-ttu-id="4ec81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ec81-121">Header</span></span>|<span data-ttu-id="4ec81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ec81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ec81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ec81-123">Authorization</span></span>|<span data-ttu-id="4ec81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ec81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ec81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ec81-125">Accept</span></span>|<span data-ttu-id="4ec81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ec81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ec81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec81-127">Request body</span></span>
<span data-ttu-id="4ec81-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4ec81-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4ec81-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4ec81-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4ec81-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ec81-130">Property</span></span>|<span data-ttu-id="4ec81-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ec81-131">Type</span></span>|<span data-ttu-id="4ec81-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ec81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ec81-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="4ec81-133">notifyManagedDevices</span></span>|<span data-ttu-id="4ec81-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ec81-134">Boolean</span></span>|<span data-ttu-id="4ec81-135">Boolean que indica se revoke notificação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="4ec81-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="4ec81-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec81-136">Response</span></span>
<span data-ttu-id="4ec81-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ec81-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ec81-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ec81-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ec81-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec81-139">Request</span></span>
<span data-ttu-id="4ec81-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ec81-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="4ec81-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec81-141">Response</span></span>
<span data-ttu-id="4ec81-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ec81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





