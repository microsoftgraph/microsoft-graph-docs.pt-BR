---
title: Excluir mobileAppTroubleshootingEvent
description: Descreve o método Delete mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41c9383524e29ff897ea255555ab663476c36659
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979876"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="dc7f4-103">Excluir mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="dc7f4-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="dc7f4-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dc7f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc7f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc7f4-107">Exclui [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="dc7f4-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc7f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc7f4-108">Prerequisites</span></span>
<span data-ttu-id="dc7f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc7f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc7f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc7f4-111">Permission type</span></span>|<span data-ttu-id="dc7f4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc7f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc7f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc7f4-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="dc7f4-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="dc7f4-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="dc7f4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc7f4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dc7f4-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="dc7f4-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="dc7f4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc7f4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dc7f4-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc7f4-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc7f4-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-119">Not supported.</span></span>|
|<span data-ttu-id="dc7f4-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc7f4-120">Application</span></span>|<span data-ttu-id="dc7f4-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc7f4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc7f4-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="dc7f4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc7f4-123">Request headers</span></span>
|<span data-ttu-id="dc7f4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc7f4-124">Header</span></span>|<span data-ttu-id="dc7f4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="dc7f4-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc7f4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc7f4-126">Authorization</span></span>|<span data-ttu-id="dc7f4-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc7f4-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc7f4-128">Accept</span></span>|<span data-ttu-id="dc7f4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="dc7f4-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc7f4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc7f4-130">Request body</span></span>
<span data-ttu-id="dc7f4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc7f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc7f4-132">Response</span></span>
<span data-ttu-id="dc7f4-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc7f4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc7f4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc7f4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc7f4-135">Request</span></span>
<span data-ttu-id="dc7f4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="dc7f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc7f4-137">Response</span></span>
<span data-ttu-id="dc7f4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc7f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




