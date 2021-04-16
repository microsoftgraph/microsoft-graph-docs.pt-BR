---
title: Excluir mobileAppTroubleshootingEvent
description: Descreve o método Delete mobileAppTroubleshootingEvent da API do Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b44012db5d7a22aa2d1ec10371e26a48731c7df1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863756"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="7d2b7-103">Excluir mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7d2b7-103">Delete mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="7d2b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d2b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d2b7-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d2b7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d2b7-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d2b7-108">Exclui um [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7d2b7-108">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d2b7-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d2b7-109">Prerequisites</span></span>
<span data-ttu-id="7d2b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d2b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d2b7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d2b7-112">Permission type</span></span>|<span data-ttu-id="7d2b7-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d2b7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d2b7-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d2b7-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="7d2b7-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7d2b7-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="7d2b7-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d2b7-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7d2b7-117">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="7d2b7-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="7d2b7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d2b7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7d2b7-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d2b7-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d2b7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-120">Not supported.</span></span>|
|<span data-ttu-id="7d2b7-121">Application</span><span class="sxs-lookup"><span data-stu-id="7d2b7-121">Application</span></span>||
|<span data-ttu-id="7d2b7-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7d2b7-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="7d2b7-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d2b7-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7d2b7-124">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="7d2b7-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="7d2b7-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d2b7-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d2b7-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d2b7-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="7d2b7-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d2b7-127">Request headers</span></span>
|<span data-ttu-id="7d2b7-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d2b7-128">Header</span></span>|<span data-ttu-id="7d2b7-129">Valor</span><span class="sxs-lookup"><span data-stu-id="7d2b7-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d2b7-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d2b7-130">Authorization</span></span>|<span data-ttu-id="7d2b7-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d2b7-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d2b7-132">Accept</span></span>|<span data-ttu-id="7d2b7-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7d2b7-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d2b7-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d2b7-134">Request body</span></span>
<span data-ttu-id="7d2b7-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d2b7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d2b7-136">Response</span></span>
<span data-ttu-id="7d2b7-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d2b7-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d2b7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d2b7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d2b7-139">Request</span></span>
<span data-ttu-id="7d2b7-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-140">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="7d2b7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d2b7-141">Response</span></span>
<span data-ttu-id="7d2b7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d2b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











