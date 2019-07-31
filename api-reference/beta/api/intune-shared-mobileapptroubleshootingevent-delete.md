---
title: Excluir mobileAppTroubleshootingEvent
description: Descreve o método Delete mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b9ae2aafe9fe740d5156f2c756a03a9905aa995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993582"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="b16b2-103">Excluir mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b16b2-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="b16b2-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b16b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b16b2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b16b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b16b2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b16b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b16b2-107">Exclui [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b16b2-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b16b2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b16b2-108">Prerequisites</span></span>
<span data-ttu-id="b16b2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b16b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b16b2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b16b2-111">Permission type</span></span>|<span data-ttu-id="b16b2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b16b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b16b2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b16b2-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="b16b2-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="b16b2-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="b16b2-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b16b2-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b16b2-116">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="b16b2-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="b16b2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b16b2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b16b2-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b16b2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b16b2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b16b2-119">Not supported.</span></span>|
|<span data-ttu-id="b16b2-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b16b2-120">Application</span></span>|<span data-ttu-id="b16b2-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b16b2-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b16b2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b16b2-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="b16b2-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b16b2-123">Request headers</span></span>
|<span data-ttu-id="b16b2-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b16b2-124">Header</span></span>|<span data-ttu-id="b16b2-125">Valor</span><span class="sxs-lookup"><span data-stu-id="b16b2-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b16b2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b16b2-126">Authorization</span></span>|<span data-ttu-id="b16b2-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b16b2-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b16b2-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b16b2-128">Accept</span></span>|<span data-ttu-id="b16b2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b16b2-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b16b2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b16b2-130">Request body</span></span>
<span data-ttu-id="b16b2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b16b2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b16b2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b16b2-132">Response</span></span>
<span data-ttu-id="b16b2-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b16b2-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b16b2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b16b2-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b16b2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b16b2-135">Request</span></span>
<span data-ttu-id="b16b2-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b16b2-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="b16b2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b16b2-137">Response</span></span>
<span data-ttu-id="b16b2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b16b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




