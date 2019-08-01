---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a248725d5e46358ba4b4434ae55a76dd1592e69d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002458"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="27cc7-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="27cc7-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="27cc7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27cc7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27cc7-105">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="27cc7-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27cc7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27cc7-106">Prerequisites</span></span>
<span data-ttu-id="27cc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27cc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27cc7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27cc7-109">Permission type</span></span>|<span data-ttu-id="27cc7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27cc7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27cc7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27cc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27cc7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27cc7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27cc7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27cc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27cc7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27cc7-114">Not supported.</span></span>|
|<span data-ttu-id="27cc7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27cc7-115">Application</span></span>|<span data-ttu-id="27cc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27cc7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27cc7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27cc7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="27cc7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27cc7-118">Request headers</span></span>
|<span data-ttu-id="27cc7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27cc7-119">Header</span></span>|<span data-ttu-id="27cc7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="27cc7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27cc7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="27cc7-121">Authorization</span></span>|<span data-ttu-id="27cc7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27cc7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27cc7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27cc7-123">Accept</span></span>|<span data-ttu-id="27cc7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27cc7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27cc7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27cc7-125">Request body</span></span>
<span data-ttu-id="27cc7-126">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="27cc7-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="27cc7-127">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="27cc7-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="27cc7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27cc7-128">Property</span></span>|<span data-ttu-id="27cc7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="27cc7-129">Type</span></span>|<span data-ttu-id="27cc7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="27cc7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27cc7-131">id</span><span class="sxs-lookup"><span data-stu-id="27cc7-131">id</span></span>|<span data-ttu-id="27cc7-132">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-132">String</span></span>|<span data-ttu-id="27cc7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27cc7-133">Key of the entity.</span></span> <span data-ttu-id="27cc7-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="27cc7-135">displayName</span></span>|<span data-ttu-id="27cc7-136">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-136">String</span></span>|<span data-ttu-id="27cc7-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="27cc7-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="27cc7-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-139">descrição</span><span class="sxs-lookup"><span data-stu-id="27cc7-139">description</span></span>|<span data-ttu-id="27cc7-140">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-140">String</span></span>|<span data-ttu-id="27cc7-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-141">The description of the app.</span></span> <span data-ttu-id="27cc7-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-143">publicador</span><span class="sxs-lookup"><span data-stu-id="27cc7-143">publisher</span></span>|<span data-ttu-id="27cc7-144">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-144">String</span></span>|<span data-ttu-id="27cc7-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-145">The publisher of the app.</span></span> <span data-ttu-id="27cc7-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="27cc7-147">largeIcon</span></span>|[<span data-ttu-id="27cc7-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="27cc7-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="27cc7-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="27cc7-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="27cc7-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27cc7-151">createdDateTime</span></span>|<span data-ttu-id="27cc7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cc7-152">DateTimeOffset</span></span>|<span data-ttu-id="27cc7-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-153">The date and time the app was created.</span></span> <span data-ttu-id="27cc7-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27cc7-155">lastModifiedDateTime</span></span>|<span data-ttu-id="27cc7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cc7-156">DateTimeOffset</span></span>|<span data-ttu-id="27cc7-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="27cc7-157">The date and time the app was last modified.</span></span> <span data-ttu-id="27cc7-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="27cc7-159">isFeatured</span></span>|<span data-ttu-id="27cc7-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cc7-160">Boolean</span></span>|<span data-ttu-id="27cc7-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="27cc7-162">privacyInformationUrl</span></span>|<span data-ttu-id="27cc7-163">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-163">String</span></span>|<span data-ttu-id="27cc7-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="27cc7-164">The privacy statement Url.</span></span> <span data-ttu-id="27cc7-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="27cc7-166">informationUrl</span></span>|<span data-ttu-id="27cc7-167">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-167">String</span></span>|<span data-ttu-id="27cc7-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="27cc7-168">The more information Url.</span></span> <span data-ttu-id="27cc7-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-170">owner</span><span class="sxs-lookup"><span data-stu-id="27cc7-170">owner</span></span>|<span data-ttu-id="27cc7-171">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-171">String</span></span>|<span data-ttu-id="27cc7-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-172">The owner of the app.</span></span> <span data-ttu-id="27cc7-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-174">developer</span><span class="sxs-lookup"><span data-stu-id="27cc7-174">developer</span></span>|<span data-ttu-id="27cc7-175">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-175">String</span></span>|<span data-ttu-id="27cc7-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-176">The developer of the app.</span></span> <span data-ttu-id="27cc7-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-178">notes</span><span class="sxs-lookup"><span data-stu-id="27cc7-178">notes</span></span>|<span data-ttu-id="27cc7-179">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-179">String</span></span>|<span data-ttu-id="27cc7-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-180">Notes for the app.</span></span> <span data-ttu-id="27cc7-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cc7-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="27cc7-182">publishingState</span></span>|[<span data-ttu-id="27cc7-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="27cc7-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="27cc7-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-184">The publishing state for the app.</span></span> <span data-ttu-id="27cc7-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="27cc7-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="27cc7-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="27cc7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="27cc7-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="27cc7-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="27cc7-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="27cc7-188">appAvailability</span></span>|[<span data-ttu-id="27cc7-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="27cc7-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="27cc7-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-190">The Application's availability.</span></span> <span data-ttu-id="27cc7-191">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="27cc7-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="27cc7-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="27cc7-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="27cc7-193">version</span><span class="sxs-lookup"><span data-stu-id="27cc7-193">version</span></span>|<span data-ttu-id="27cc7-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27cc7-194">String</span></span>|<span data-ttu-id="27cc7-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27cc7-195">The Application's version.</span></span> <span data-ttu-id="27cc7-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="27cc7-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="27cc7-197">committedContentVersion</span></span>|<span data-ttu-id="27cc7-198">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-198">String</span></span>|<span data-ttu-id="27cc7-199">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="27cc7-199">The internal committed content version.</span></span> <span data-ttu-id="27cc7-200">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="27cc7-201">fileName</span><span class="sxs-lookup"><span data-stu-id="27cc7-201">fileName</span></span>|<span data-ttu-id="27cc7-202">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-202">String</span></span>|<span data-ttu-id="27cc7-203">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="27cc7-203">The name of the main Lob application file.</span></span> <span data-ttu-id="27cc7-204">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="27cc7-205">size</span><span class="sxs-lookup"><span data-stu-id="27cc7-205">size</span></span>|<span data-ttu-id="27cc7-206">Int64</span><span class="sxs-lookup"><span data-stu-id="27cc7-206">Int64</span></span>|<span data-ttu-id="27cc7-207">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="27cc7-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="27cc7-208">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="27cc7-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="27cc7-209">packageId</span><span class="sxs-lookup"><span data-stu-id="27cc7-209">packageId</span></span>|<span data-ttu-id="27cc7-210">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-210">String</span></span>|<span data-ttu-id="27cc7-211">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="27cc7-211">The package identifier.</span></span>|
|<span data-ttu-id="27cc7-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="27cc7-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="27cc7-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="27cc7-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="27cc7-214">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="27cc7-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="27cc7-215">versionName</span><span class="sxs-lookup"><span data-stu-id="27cc7-215">versionName</span></span>|<span data-ttu-id="27cc7-216">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-216">String</span></span>|<span data-ttu-id="27cc7-217">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="27cc7-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="27cc7-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="27cc7-218">versionCode</span></span>|<span data-ttu-id="27cc7-219">String</span><span class="sxs-lookup"><span data-stu-id="27cc7-219">String</span></span>|<span data-ttu-id="27cc7-220">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="27cc7-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="27cc7-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="27cc7-221">Response</span></span>
<span data-ttu-id="27cc7-222">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27cc7-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27cc7-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27cc7-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="27cc7-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27cc7-224">Request</span></span>
<span data-ttu-id="27cc7-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27cc7-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="27cc7-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="27cc7-226">Response</span></span>
<span data-ttu-id="27cc7-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27cc7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



