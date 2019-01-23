---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aa276827960b0ac0b73489402ac7ba309c58c098
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412923"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="ae89d-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="ae89d-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="ae89d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae89d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae89d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae89d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae89d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ae89d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae89d-107">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae89d-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae89d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae89d-108">Prerequisites</span></span>
<span data-ttu-id="ae89d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae89d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae89d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae89d-111">Permission type</span></span>|<span data-ttu-id="ae89d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae89d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae89d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae89d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae89d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae89d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae89d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae89d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae89d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae89d-116">Not supported.</span></span>|
|<span data-ttu-id="ae89d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae89d-117">Application</span></span>|<span data-ttu-id="ae89d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae89d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae89d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae89d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ae89d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae89d-120">Request headers</span></span>
|<span data-ttu-id="ae89d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae89d-121">Header</span></span>|<span data-ttu-id="ae89d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae89d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae89d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae89d-123">Authorization</span></span>|<span data-ttu-id="ae89d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae89d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae89d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae89d-125">Accept</span></span>|<span data-ttu-id="ae89d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae89d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae89d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae89d-127">Request body</span></span>
<span data-ttu-id="ae89d-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae89d-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="ae89d-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae89d-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="ae89d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae89d-130">Property</span></span>|<span data-ttu-id="ae89d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae89d-131">Type</span></span>|<span data-ttu-id="ae89d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae89d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae89d-133">id</span><span class="sxs-lookup"><span data-stu-id="ae89d-133">id</span></span>|<span data-ttu-id="ae89d-134">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-134">String</span></span>|<span data-ttu-id="ae89d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ae89d-135">Key of the entity.</span></span> <span data-ttu-id="ae89d-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ae89d-137">displayName</span></span>|<span data-ttu-id="ae89d-138">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-138">String</span></span>|<span data-ttu-id="ae89d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ae89d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ae89d-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-141">description</span><span class="sxs-lookup"><span data-stu-id="ae89d-141">description</span></span>|<span data-ttu-id="ae89d-142">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-142">String</span></span>|<span data-ttu-id="ae89d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-143">The description of the app.</span></span> <span data-ttu-id="ae89d-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ae89d-145">publisher</span></span>|<span data-ttu-id="ae89d-146">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-146">String</span></span>|<span data-ttu-id="ae89d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-147">The publisher of the app.</span></span> <span data-ttu-id="ae89d-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ae89d-149">largeIcon</span></span>|[<span data-ttu-id="ae89d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ae89d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ae89d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ae89d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ae89d-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae89d-153">createdDateTime</span></span>|<span data-ttu-id="ae89d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae89d-154">DateTimeOffset</span></span>|<span data-ttu-id="ae89d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-155">The date and time the app was created.</span></span> <span data-ttu-id="ae89d-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae89d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ae89d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae89d-158">DateTimeOffset</span></span>|<span data-ttu-id="ae89d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ae89d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ae89d-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ae89d-161">isFeatured</span></span>|<span data-ttu-id="ae89d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae89d-162">Boolean</span></span>|<span data-ttu-id="ae89d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ae89d-164">privacyInformationUrl</span></span>|<span data-ttu-id="ae89d-165">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-165">String</span></span>|<span data-ttu-id="ae89d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ae89d-166">The privacy statement Url.</span></span> <span data-ttu-id="ae89d-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ae89d-168">informationUrl</span></span>|<span data-ttu-id="ae89d-169">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-169">String</span></span>|<span data-ttu-id="ae89d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ae89d-170">The more information Url.</span></span> <span data-ttu-id="ae89d-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-172">owner</span><span class="sxs-lookup"><span data-stu-id="ae89d-172">owner</span></span>|<span data-ttu-id="ae89d-173">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-173">String</span></span>|<span data-ttu-id="ae89d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-174">The owner of the app.</span></span> <span data-ttu-id="ae89d-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-176">developer</span><span class="sxs-lookup"><span data-stu-id="ae89d-176">developer</span></span>|<span data-ttu-id="ae89d-177">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-177">String</span></span>|<span data-ttu-id="ae89d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-178">The developer of the app.</span></span> <span data-ttu-id="ae89d-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-180">Observações</span><span class="sxs-lookup"><span data-stu-id="ae89d-180">notes</span></span>|<span data-ttu-id="ae89d-181">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-181">String</span></span>|<span data-ttu-id="ae89d-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-182">Notes for the app.</span></span> <span data-ttu-id="ae89d-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ae89d-184">uploadState</span></span>|<span data-ttu-id="ae89d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ae89d-185">Int32</span></span>|<span data-ttu-id="ae89d-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="ae89d-186">The upload state.</span></span> <span data-ttu-id="ae89d-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ae89d-188">publishingState</span></span>|[<span data-ttu-id="ae89d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ae89d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ae89d-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-190">The publishing state for the app.</span></span> <span data-ttu-id="ae89d-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ae89d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ae89d-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae89d-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ae89d-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ae89d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ae89d-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ae89d-194">isAssigned</span></span>|<span data-ttu-id="ae89d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae89d-195">Boolean</span></span>|<span data-ttu-id="ae89d-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ae89d-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae89d-198">roleScopeTagIds</span></span>|<span data-ttu-id="ae89d-199">String collection</span><span class="sxs-lookup"><span data-stu-id="ae89d-199">String collection</span></span>|<span data-ttu-id="ae89d-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ae89d-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ae89d-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae89d-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ae89d-202">appAvailability</span></span>|[<span data-ttu-id="ae89d-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ae89d-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ae89d-204">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-204">The Application's availability.</span></span> <span data-ttu-id="ae89d-205">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae89d-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ae89d-206">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ae89d-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ae89d-207">version</span><span class="sxs-lookup"><span data-stu-id="ae89d-207">version</span></span>|<span data-ttu-id="ae89d-208">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-208">String</span></span>|<span data-ttu-id="ae89d-209">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae89d-209">The Application's version.</span></span> <span data-ttu-id="ae89d-210">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ae89d-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ae89d-211">committedContentVersion</span></span>|<span data-ttu-id="ae89d-212">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-212">String</span></span>|<span data-ttu-id="ae89d-213">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ae89d-213">The internal committed content version.</span></span> <span data-ttu-id="ae89d-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae89d-215">fileName</span><span class="sxs-lookup"><span data-stu-id="ae89d-215">fileName</span></span>|<span data-ttu-id="ae89d-216">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-216">String</span></span>|<span data-ttu-id="ae89d-217">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ae89d-217">The name of the main Lob application file.</span></span> <span data-ttu-id="ae89d-218">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae89d-219">size</span><span class="sxs-lookup"><span data-stu-id="ae89d-219">size</span></span>|<span data-ttu-id="ae89d-220">Int64</span><span class="sxs-lookup"><span data-stu-id="ae89d-220">Int64</span></span>|<span data-ttu-id="ae89d-221">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ae89d-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="ae89d-222">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae89d-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae89d-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="ae89d-223">bundleId</span></span>|<span data-ttu-id="ae89d-224">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-224">String</span></span>|<span data-ttu-id="ae89d-225">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ae89d-225">The Identity Name.</span></span>|
|<span data-ttu-id="ae89d-226">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ae89d-226">applicableDeviceType</span></span>|[<span data-ttu-id="ae89d-227">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ae89d-227">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ae89d-228">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="ae89d-228">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ae89d-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae89d-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ae89d-230">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae89d-230">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ae89d-231">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ae89d-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ae89d-232">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ae89d-232">expirationDateTime</span></span>|<span data-ttu-id="ae89d-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae89d-233">DateTimeOffset</span></span>|<span data-ttu-id="ae89d-234">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="ae89d-234">The expiration time.</span></span>|
|<span data-ttu-id="ae89d-235">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ae89d-235">versionNumber</span></span>|<span data-ttu-id="ae89d-236">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-236">String</span></span>|<span data-ttu-id="ae89d-237">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ae89d-237">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae89d-238">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ae89d-238">buildNumber</span></span>|<span data-ttu-id="ae89d-239">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-239">String</span></span>|<span data-ttu-id="ae89d-240">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ae89d-240">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae89d-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ae89d-241">identityVersion</span></span>|<span data-ttu-id="ae89d-242">String</span><span class="sxs-lookup"><span data-stu-id="ae89d-242">String</span></span>|<span data-ttu-id="ae89d-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ae89d-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ae89d-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae89d-244">Response</span></span>
<span data-ttu-id="ae89d-245">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae89d-245">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae89d-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae89d-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae89d-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae89d-247">Request</span></span>
<span data-ttu-id="ae89d-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae89d-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ae89d-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae89d-249">Response</span></span>
<span data-ttu-id="ae89d-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae89d-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




