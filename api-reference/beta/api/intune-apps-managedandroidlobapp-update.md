---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7fa0ace9f4e1235b5ca63ee9c7249d7f667c8b2e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394639"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="ae630-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="ae630-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="ae630-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae630-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae630-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae630-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae630-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ae630-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae630-107">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae630-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae630-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae630-108">Prerequisites</span></span>
<span data-ttu-id="ae630-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae630-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae630-111">Permission type</span></span>|<span data-ttu-id="ae630-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae630-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae630-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae630-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae630-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae630-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae630-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae630-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae630-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae630-116">Not supported.</span></span>|
|<span data-ttu-id="ae630-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae630-117">Application</span></span>|<span data-ttu-id="ae630-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae630-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae630-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae630-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ae630-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae630-120">Request headers</span></span>
|<span data-ttu-id="ae630-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae630-121">Header</span></span>|<span data-ttu-id="ae630-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae630-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae630-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae630-123">Authorization</span></span>|<span data-ttu-id="ae630-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae630-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae630-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae630-125">Accept</span></span>|<span data-ttu-id="ae630-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae630-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae630-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae630-127">Request body</span></span>
<span data-ttu-id="ae630-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae630-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="ae630-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae630-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="ae630-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae630-130">Property</span></span>|<span data-ttu-id="ae630-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae630-131">Type</span></span>|<span data-ttu-id="ae630-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae630-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae630-133">id</span><span class="sxs-lookup"><span data-stu-id="ae630-133">id</span></span>|<span data-ttu-id="ae630-134">String</span><span class="sxs-lookup"><span data-stu-id="ae630-134">String</span></span>|<span data-ttu-id="ae630-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ae630-135">Key of the entity.</span></span> <span data-ttu-id="ae630-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ae630-137">displayName</span></span>|<span data-ttu-id="ae630-138">String</span><span class="sxs-lookup"><span data-stu-id="ae630-138">String</span></span>|<span data-ttu-id="ae630-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ae630-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ae630-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-141">description</span><span class="sxs-lookup"><span data-stu-id="ae630-141">description</span></span>|<span data-ttu-id="ae630-142">String</span><span class="sxs-lookup"><span data-stu-id="ae630-142">String</span></span>|<span data-ttu-id="ae630-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-143">The description of the app.</span></span> <span data-ttu-id="ae630-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ae630-145">publisher</span></span>|<span data-ttu-id="ae630-146">String</span><span class="sxs-lookup"><span data-stu-id="ae630-146">String</span></span>|<span data-ttu-id="ae630-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-147">The publisher of the app.</span></span> <span data-ttu-id="ae630-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ae630-149">largeIcon</span></span>|[<span data-ttu-id="ae630-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ae630-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ae630-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ae630-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ae630-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae630-153">createdDateTime</span></span>|<span data-ttu-id="ae630-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae630-154">DateTimeOffset</span></span>|<span data-ttu-id="ae630-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-155">The date and time the app was created.</span></span> <span data-ttu-id="ae630-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae630-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ae630-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae630-158">DateTimeOffset</span></span>|<span data-ttu-id="ae630-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ae630-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ae630-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ae630-161">isFeatured</span></span>|<span data-ttu-id="ae630-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae630-162">Boolean</span></span>|<span data-ttu-id="ae630-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ae630-164">privacyInformationUrl</span></span>|<span data-ttu-id="ae630-165">String</span><span class="sxs-lookup"><span data-stu-id="ae630-165">String</span></span>|<span data-ttu-id="ae630-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ae630-166">The privacy statement Url.</span></span> <span data-ttu-id="ae630-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ae630-168">informationUrl</span></span>|<span data-ttu-id="ae630-169">String</span><span class="sxs-lookup"><span data-stu-id="ae630-169">String</span></span>|<span data-ttu-id="ae630-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ae630-170">The more information Url.</span></span> <span data-ttu-id="ae630-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-172">owner</span><span class="sxs-lookup"><span data-stu-id="ae630-172">owner</span></span>|<span data-ttu-id="ae630-173">String</span><span class="sxs-lookup"><span data-stu-id="ae630-173">String</span></span>|<span data-ttu-id="ae630-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ae630-174">The owner of the app.</span></span> <span data-ttu-id="ae630-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-176">developer</span><span class="sxs-lookup"><span data-stu-id="ae630-176">developer</span></span>|<span data-ttu-id="ae630-177">String</span><span class="sxs-lookup"><span data-stu-id="ae630-177">String</span></span>|<span data-ttu-id="ae630-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-178">The developer of the app.</span></span> <span data-ttu-id="ae630-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-180">Observações</span><span class="sxs-lookup"><span data-stu-id="ae630-180">notes</span></span>|<span data-ttu-id="ae630-181">String</span><span class="sxs-lookup"><span data-stu-id="ae630-181">String</span></span>|<span data-ttu-id="ae630-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-182">Notes for the app.</span></span> <span data-ttu-id="ae630-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ae630-184">uploadState</span></span>|<span data-ttu-id="ae630-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ae630-185">Int32</span></span>|<span data-ttu-id="ae630-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="ae630-186">The upload state.</span></span> <span data-ttu-id="ae630-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ae630-188">publishingState</span></span>|[<span data-ttu-id="ae630-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ae630-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ae630-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-190">The publishing state for the app.</span></span> <span data-ttu-id="ae630-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ae630-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ae630-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae630-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ae630-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ae630-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ae630-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ae630-194">isAssigned</span></span>|<span data-ttu-id="ae630-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae630-195">Boolean</span></span>|<span data-ttu-id="ae630-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ae630-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ae630-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae630-198">roleScopeTagIds</span></span>|<span data-ttu-id="ae630-199">String collection</span><span class="sxs-lookup"><span data-stu-id="ae630-199">String collection</span></span>|<span data-ttu-id="ae630-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ae630-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ae630-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ae630-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ae630-202">appAvailability</span></span>|[<span data-ttu-id="ae630-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ae630-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ae630-204">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-204">The Application's availability.</span></span> <span data-ttu-id="ae630-205">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae630-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ae630-206">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ae630-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ae630-207">version</span><span class="sxs-lookup"><span data-stu-id="ae630-207">version</span></span>|<span data-ttu-id="ae630-208">String</span><span class="sxs-lookup"><span data-stu-id="ae630-208">String</span></span>|<span data-ttu-id="ae630-209">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae630-209">The Application's version.</span></span> <span data-ttu-id="ae630-210">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ae630-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ae630-211">committedContentVersion</span></span>|<span data-ttu-id="ae630-212">String</span><span class="sxs-lookup"><span data-stu-id="ae630-212">String</span></span>|<span data-ttu-id="ae630-213">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ae630-213">The internal committed content version.</span></span> <span data-ttu-id="ae630-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae630-215">fileName</span><span class="sxs-lookup"><span data-stu-id="ae630-215">fileName</span></span>|<span data-ttu-id="ae630-216">String</span><span class="sxs-lookup"><span data-stu-id="ae630-216">String</span></span>|<span data-ttu-id="ae630-217">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ae630-217">The name of the main Lob application file.</span></span> <span data-ttu-id="ae630-218">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae630-219">size</span><span class="sxs-lookup"><span data-stu-id="ae630-219">size</span></span>|<span data-ttu-id="ae630-220">Int64</span><span class="sxs-lookup"><span data-stu-id="ae630-220">Int64</span></span>|<span data-ttu-id="ae630-221">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ae630-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="ae630-222">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ae630-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae630-223">packageId</span><span class="sxs-lookup"><span data-stu-id="ae630-223">packageId</span></span>|<span data-ttu-id="ae630-224">String</span><span class="sxs-lookup"><span data-stu-id="ae630-224">String</span></span>|<span data-ttu-id="ae630-225">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="ae630-225">The package identifier.</span></span>|
|<span data-ttu-id="ae630-226">identityName</span><span class="sxs-lookup"><span data-stu-id="ae630-226">identityName</span></span>|<span data-ttu-id="ae630-227">String</span><span class="sxs-lookup"><span data-stu-id="ae630-227">String</span></span>|<span data-ttu-id="ae630-228">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ae630-228">The Identity Name.</span></span>|
|<span data-ttu-id="ae630-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae630-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ae630-230">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae630-230">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ae630-231">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ae630-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ae630-232">versionName</span><span class="sxs-lookup"><span data-stu-id="ae630-232">versionName</span></span>|<span data-ttu-id="ae630-233">String</span><span class="sxs-lookup"><span data-stu-id="ae630-233">String</span></span>|<span data-ttu-id="ae630-234">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ae630-234">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae630-235">versionCode</span><span class="sxs-lookup"><span data-stu-id="ae630-235">versionCode</span></span>|<span data-ttu-id="ae630-236">String</span><span class="sxs-lookup"><span data-stu-id="ae630-236">String</span></span>|<span data-ttu-id="ae630-237">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ae630-237">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae630-238">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ae630-238">identityVersion</span></span>|<span data-ttu-id="ae630-239">String</span><span class="sxs-lookup"><span data-stu-id="ae630-239">String</span></span>|<span data-ttu-id="ae630-240">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ae630-240">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ae630-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae630-241">Response</span></span>
<span data-ttu-id="ae630-242">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae630-242">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae630-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae630-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae630-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae630-244">Request</span></span>
<span data-ttu-id="ae630-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae630-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1464

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ae630-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae630-246">Response</span></span>
<span data-ttu-id="ae630-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae630-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1636

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




