---
title: ação de revokeUserLicense
description: REVOKE atribuído iOS VPP licença de usuário para fornecido app.
ms.openlocfilehash: 0222623ba5e1f3de0122a632a3ea9554bbd2c0ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033948"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="cfc9b-103">ação de revokeUserLicense</span><span class="sxs-lookup"><span data-stu-id="cfc9b-103">revokeUserLicense action</span></span>

> <span data-ttu-id="cfc9b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfc9b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfc9b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfc9b-107">REVOKE atribuído iOS VPP licença de usuário para fornecido app.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-107">Revoke assigned iOS VPP user license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cfc9b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfc9b-108">Prerequisites</span></span>
<span data-ttu-id="cfc9b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfc9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfc9b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfc9b-111">Permission type</span></span>|<span data-ttu-id="cfc9b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfc9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfc9b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfc9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfc9b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfc9b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cfc9b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfc9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfc9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-116">Not supported.</span></span>|
|<span data-ttu-id="cfc9b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfc9b-117">Application</span></span>|<span data-ttu-id="cfc9b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfc9b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="cfc9b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc9b-120">Request headers</span></span>
|<span data-ttu-id="cfc9b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfc9b-121">Header</span></span>|<span data-ttu-id="cfc9b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cfc9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfc9b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfc9b-123">Authorization</span></span>|<span data-ttu-id="cfc9b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfc9b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cfc9b-125">Accept</span></span>|<span data-ttu-id="cfc9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfc9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfc9b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc9b-127">Request body</span></span>
<span data-ttu-id="cfc9b-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cfc9b-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cfc9b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfc9b-130">Property</span></span>|<span data-ttu-id="cfc9b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfc9b-131">Type</span></span>|<span data-ttu-id="cfc9b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfc9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfc9b-133">userId</span><span class="sxs-lookup"><span data-stu-id="cfc9b-133">userId</span></span>|<span data-ttu-id="cfc9b-134">String</span><span class="sxs-lookup"><span data-stu-id="cfc9b-134">String</span></span>|<span data-ttu-id="cfc9b-135">ID de usuário para quem a licença de aplicativo atribuídas é a ser revogado</span><span class="sxs-lookup"><span data-stu-id="cfc9b-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="cfc9b-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="cfc9b-136">notifyManagedDevices</span></span>|<span data-ttu-id="cfc9b-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="cfc9b-137">Boolean</span></span>|<span data-ttu-id="cfc9b-138">Boolean que indica se revoke notificação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="cfc9b-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="cfc9b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc9b-139">Response</span></span>
<span data-ttu-id="cfc9b-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cfc9b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfc9b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="cfc9b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc9b-142">Request</span></span>
<span data-ttu-id="cfc9b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="cfc9b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc9b-144">Response</span></span>
<span data-ttu-id="cfc9b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfc9b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





