---
title: ação de revokeUserLicense
description: REVOKE atribuído iOS VPP licença de usuário para fornecido app.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f94cf25824d6e81c609c634c03f5e607fa75dfb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417844"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="9fd38-103">ação de revokeUserLicense</span><span class="sxs-lookup"><span data-stu-id="9fd38-103">revokeUserLicense action</span></span>

> <span data-ttu-id="9fd38-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9fd38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9fd38-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9fd38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fd38-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9fd38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fd38-107">REVOKE atribuído iOS VPP licença de usuário para fornecido app.</span><span class="sxs-lookup"><span data-stu-id="9fd38-107">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fd38-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fd38-108">Prerequisites</span></span>
<span data-ttu-id="9fd38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9fd38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9fd38-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fd38-111">Permission type</span></span>|<span data-ttu-id="9fd38-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fd38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fd38-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fd38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fd38-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd38-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fd38-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fd38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fd38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd38-116">Not supported.</span></span>|
|<span data-ttu-id="9fd38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fd38-117">Application</span></span>|<span data-ttu-id="9fd38-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fd38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="9fd38-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd38-120">Request headers</span></span>
|<span data-ttu-id="9fd38-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fd38-121">Header</span></span>|<span data-ttu-id="9fd38-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9fd38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fd38-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fd38-123">Authorization</span></span>|<span data-ttu-id="9fd38-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fd38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fd38-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fd38-125">Accept</span></span>|<span data-ttu-id="9fd38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fd38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fd38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd38-127">Request body</span></span>
<span data-ttu-id="9fd38-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9fd38-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9fd38-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9fd38-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9fd38-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fd38-130">Property</span></span>|<span data-ttu-id="9fd38-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd38-131">Type</span></span>|<span data-ttu-id="9fd38-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fd38-133">userId</span><span class="sxs-lookup"><span data-stu-id="9fd38-133">userId</span></span>|<span data-ttu-id="9fd38-134">String</span><span class="sxs-lookup"><span data-stu-id="9fd38-134">String</span></span>|<span data-ttu-id="9fd38-135">ID de usuário para quem a licença de aplicativo atribuídas é a ser revogado</span><span class="sxs-lookup"><span data-stu-id="9fd38-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="9fd38-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="9fd38-136">notifyManagedDevices</span></span>|<span data-ttu-id="9fd38-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fd38-137">Boolean</span></span>|<span data-ttu-id="9fd38-138">Boolean que indica se revoke notificação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="9fd38-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="9fd38-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd38-139">Response</span></span>
<span data-ttu-id="9fd38-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9fd38-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9fd38-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fd38-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fd38-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd38-142">Request</span></span>
<span data-ttu-id="9fd38-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fd38-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="9fd38-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd38-144">Response</span></span>
<span data-ttu-id="9fd38-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fd38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




