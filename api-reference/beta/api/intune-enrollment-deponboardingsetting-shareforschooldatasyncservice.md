---
title: ação de shareForSchoolDataSyncService
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5bac5f17089016e3f300d9f4736f965c4f0a25a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425257"
---
# <a name="shareforschooldatasyncservice-action"></a><span data-ttu-id="a6e45-103">ação de shareForSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="a6e45-103">shareForSchoolDataSyncService action</span></span>

> <span data-ttu-id="a6e45-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6e45-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6e45-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6e45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6e45-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a6e45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6e45-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6e45-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6e45-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6e45-108">Prerequisites</span></span>
<span data-ttu-id="a6e45-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6e45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6e45-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6e45-111">Permission type</span></span>|<span data-ttu-id="a6e45-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6e45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6e45-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6e45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6e45-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e45-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6e45-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6e45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6e45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6e45-116">Not supported.</span></span>|
|<span data-ttu-id="a6e45-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6e45-117">Application</span></span>|<span data-ttu-id="a6e45-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6e45-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6e45-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/shareForSchoolDataSyncService
```

## <a name="request-headers"></a><span data-ttu-id="a6e45-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e45-120">Request headers</span></span>
|<span data-ttu-id="a6e45-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6e45-121">Header</span></span>|<span data-ttu-id="a6e45-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6e45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6e45-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6e45-123">Authorization</span></span>|<span data-ttu-id="a6e45-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6e45-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6e45-125">Accept</span></span>|<span data-ttu-id="a6e45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6e45-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e45-127">Request body</span></span>
<span data-ttu-id="a6e45-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6e45-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6e45-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e45-129">Response</span></span>
<span data-ttu-id="a6e45-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a6e45-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6e45-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6e45-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6e45-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e45-132">Request</span></span>
<span data-ttu-id="a6e45-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6e45-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/shareForSchoolDataSyncService
```

### <a name="response"></a><span data-ttu-id="a6e45-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e45-134">Response</span></span>
<span data-ttu-id="a6e45-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6e45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




