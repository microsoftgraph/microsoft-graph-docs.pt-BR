---
title: Ação targetApps
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 957a1003554299e3dec52b05838fe58e0b2eea4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882065"
---
# <a name="targetapps-action"></a><span data-ttu-id="1718b-103">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="1718b-103">targetApps action</span></span>

> <span data-ttu-id="1718b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1718b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1718b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1718b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1718b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1718b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1718b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1718b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1718b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1718b-108">Prerequisites</span></span>
<span data-ttu-id="1718b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1718b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1718b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1718b-111">Permission type</span></span>|<span data-ttu-id="1718b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1718b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1718b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1718b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1718b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1718b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1718b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1718b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1718b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1718b-116">Not supported.</span></span>|
|<span data-ttu-id="1718b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1718b-117">Application</span></span>|<span data-ttu-id="1718b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1718b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1718b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1718b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="1718b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1718b-120">Request headers</span></span>
|<span data-ttu-id="1718b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1718b-121">Header</span></span>|<span data-ttu-id="1718b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1718b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1718b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1718b-123">Authorization</span></span>|<span data-ttu-id="1718b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1718b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1718b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1718b-125">Accept</span></span>|<span data-ttu-id="1718b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1718b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1718b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1718b-127">Request body</span></span>
<span data-ttu-id="1718b-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1718b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1718b-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1718b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1718b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1718b-130">Property</span></span>|<span data-ttu-id="1718b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1718b-131">Type</span></span>|<span data-ttu-id="1718b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1718b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1718b-133">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="1718b-133">apps</span></span>|<span data-ttu-id="1718b-134">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1718b-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="1718b-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1718b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1718b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1718b-136">Response</span></span>
<span data-ttu-id="1718b-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1718b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1718b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1718b-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="1718b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1718b-139">Request</span></span>
<span data-ttu-id="1718b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1718b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1718b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1718b-141">Response</span></span>
<span data-ttu-id="1718b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1718b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





