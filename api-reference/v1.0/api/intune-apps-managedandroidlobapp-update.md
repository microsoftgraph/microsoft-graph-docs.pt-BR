---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebf6faafb5d6dc5e864513f33a7368029688e753
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516416"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="05a47-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="05a47-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="05a47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05a47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05a47-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05a47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05a47-106">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="05a47-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05a47-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05a47-107">Prerequisites</span></span>
<span data-ttu-id="05a47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05a47-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05a47-110">Permission type</span></span>|<span data-ttu-id="05a47-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05a47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05a47-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05a47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05a47-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a47-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05a47-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05a47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05a47-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05a47-115">Not supported.</span></span>|
|<span data-ttu-id="05a47-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05a47-116">Application</span></span>|<span data-ttu-id="05a47-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05a47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05a47-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05a47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="05a47-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05a47-119">Request headers</span></span>
|<span data-ttu-id="05a47-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05a47-120">Header</span></span>|<span data-ttu-id="05a47-121">Valor</span><span class="sxs-lookup"><span data-stu-id="05a47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05a47-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05a47-122">Authorization</span></span>|<span data-ttu-id="05a47-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05a47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05a47-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05a47-124">Accept</span></span>|<span data-ttu-id="05a47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05a47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05a47-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05a47-126">Request body</span></span>
<span data-ttu-id="05a47-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="05a47-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="05a47-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="05a47-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="05a47-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05a47-129">Property</span></span>|<span data-ttu-id="05a47-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="05a47-130">Type</span></span>|<span data-ttu-id="05a47-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="05a47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05a47-132">id</span><span class="sxs-lookup"><span data-stu-id="05a47-132">id</span></span>|<span data-ttu-id="05a47-133">String</span><span class="sxs-lookup"><span data-stu-id="05a47-133">String</span></span>|<span data-ttu-id="05a47-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05a47-134">Key of the entity.</span></span> <span data-ttu-id="05a47-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-136">displayName</span><span class="sxs-lookup"><span data-stu-id="05a47-136">displayName</span></span>|<span data-ttu-id="05a47-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05a47-137">String</span></span>|<span data-ttu-id="05a47-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="05a47-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="05a47-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-140">description</span><span class="sxs-lookup"><span data-stu-id="05a47-140">description</span></span>|<span data-ttu-id="05a47-141">String</span><span class="sxs-lookup"><span data-stu-id="05a47-141">String</span></span>|<span data-ttu-id="05a47-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-142">The description of the app.</span></span> <span data-ttu-id="05a47-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-144">publicador</span><span class="sxs-lookup"><span data-stu-id="05a47-144">publisher</span></span>|<span data-ttu-id="05a47-145">String</span><span class="sxs-lookup"><span data-stu-id="05a47-145">String</span></span>|<span data-ttu-id="05a47-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-146">The publisher of the app.</span></span> <span data-ttu-id="05a47-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="05a47-148">largeIcon</span></span>|[<span data-ttu-id="05a47-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05a47-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05a47-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="05a47-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="05a47-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05a47-152">createdDateTime</span></span>|<span data-ttu-id="05a47-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05a47-153">DateTimeOffset</span></span>|<span data-ttu-id="05a47-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-154">The date and time the app was created.</span></span> <span data-ttu-id="05a47-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05a47-156">lastModifiedDateTime</span></span>|<span data-ttu-id="05a47-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05a47-157">DateTimeOffset</span></span>|<span data-ttu-id="05a47-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="05a47-158">The date and time the app was last modified.</span></span> <span data-ttu-id="05a47-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="05a47-160">isFeatured</span></span>|<span data-ttu-id="05a47-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="05a47-161">Boolean</span></span>|<span data-ttu-id="05a47-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="05a47-163">privacyInformationUrl</span></span>|<span data-ttu-id="05a47-164">String</span><span class="sxs-lookup"><span data-stu-id="05a47-164">String</span></span>|<span data-ttu-id="05a47-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="05a47-165">The privacy statement Url.</span></span> <span data-ttu-id="05a47-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="05a47-167">informationUrl</span></span>|<span data-ttu-id="05a47-168">String</span><span class="sxs-lookup"><span data-stu-id="05a47-168">String</span></span>|<span data-ttu-id="05a47-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="05a47-169">The more information Url.</span></span> <span data-ttu-id="05a47-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-171">owner</span><span class="sxs-lookup"><span data-stu-id="05a47-171">owner</span></span>|<span data-ttu-id="05a47-172">String</span><span class="sxs-lookup"><span data-stu-id="05a47-172">String</span></span>|<span data-ttu-id="05a47-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="05a47-173">The owner of the app.</span></span> <span data-ttu-id="05a47-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-175">developer</span><span class="sxs-lookup"><span data-stu-id="05a47-175">developer</span></span>|<span data-ttu-id="05a47-176">String</span><span class="sxs-lookup"><span data-stu-id="05a47-176">String</span></span>|<span data-ttu-id="05a47-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-177">The developer of the app.</span></span> <span data-ttu-id="05a47-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-179">notes</span><span class="sxs-lookup"><span data-stu-id="05a47-179">notes</span></span>|<span data-ttu-id="05a47-180">String</span><span class="sxs-lookup"><span data-stu-id="05a47-180">String</span></span>|<span data-ttu-id="05a47-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-181">Notes for the app.</span></span> <span data-ttu-id="05a47-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05a47-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="05a47-183">publishingState</span></span>|[<span data-ttu-id="05a47-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="05a47-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="05a47-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-185">The publishing state for the app.</span></span> <span data-ttu-id="05a47-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="05a47-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="05a47-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05a47-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="05a47-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="05a47-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="05a47-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="05a47-189">appAvailability</span></span>|[<span data-ttu-id="05a47-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="05a47-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="05a47-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-191">The Application's availability.</span></span> <span data-ttu-id="05a47-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="05a47-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="05a47-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="05a47-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="05a47-194">version</span><span class="sxs-lookup"><span data-stu-id="05a47-194">version</span></span>|<span data-ttu-id="05a47-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05a47-195">String</span></span>|<span data-ttu-id="05a47-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05a47-196">The Application's version.</span></span> <span data-ttu-id="05a47-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="05a47-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="05a47-198">committedContentVersion</span></span>|<span data-ttu-id="05a47-199">String</span><span class="sxs-lookup"><span data-stu-id="05a47-199">String</span></span>|<span data-ttu-id="05a47-200">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="05a47-200">The internal committed content version.</span></span> <span data-ttu-id="05a47-201">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="05a47-202">fileName</span><span class="sxs-lookup"><span data-stu-id="05a47-202">fileName</span></span>|<span data-ttu-id="05a47-203">String</span><span class="sxs-lookup"><span data-stu-id="05a47-203">String</span></span>|<span data-ttu-id="05a47-204">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="05a47-204">The name of the main Lob application file.</span></span> <span data-ttu-id="05a47-205">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="05a47-206">size</span><span class="sxs-lookup"><span data-stu-id="05a47-206">size</span></span>|<span data-ttu-id="05a47-207">Int64</span><span class="sxs-lookup"><span data-stu-id="05a47-207">Int64</span></span>|<span data-ttu-id="05a47-208">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="05a47-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="05a47-209">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="05a47-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="05a47-210">packageId</span><span class="sxs-lookup"><span data-stu-id="05a47-210">packageId</span></span>|<span data-ttu-id="05a47-211">String</span><span class="sxs-lookup"><span data-stu-id="05a47-211">String</span></span>|<span data-ttu-id="05a47-212">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="05a47-212">The package identifier.</span></span>|
|<span data-ttu-id="05a47-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="05a47-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="05a47-214">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="05a47-214">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="05a47-215">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="05a47-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="05a47-216">versionName</span><span class="sxs-lookup"><span data-stu-id="05a47-216">versionName</span></span>|<span data-ttu-id="05a47-217">String</span><span class="sxs-lookup"><span data-stu-id="05a47-217">String</span></span>|<span data-ttu-id="05a47-218">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05a47-218">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="05a47-219">versionCode</span><span class="sxs-lookup"><span data-stu-id="05a47-219">versionCode</span></span>|<span data-ttu-id="05a47-220">String</span><span class="sxs-lookup"><span data-stu-id="05a47-220">String</span></span>|<span data-ttu-id="05a47-221">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="05a47-221">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="05a47-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="05a47-222">Response</span></span>
<span data-ttu-id="05a47-223">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05a47-223">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05a47-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05a47-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="05a47-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05a47-225">Request</span></span>
<span data-ttu-id="05a47-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05a47-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1153

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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="05a47-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="05a47-227">Response</span></span>
<span data-ttu-id="05a47-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05a47-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




