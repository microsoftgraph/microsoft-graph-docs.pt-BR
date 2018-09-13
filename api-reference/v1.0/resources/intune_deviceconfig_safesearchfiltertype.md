# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="e40a6-101">tipo enumerado safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="e40a6-101">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="e40a6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e40a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e40a6-103">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessário</span><span class="sxs-lookup"><span data-stu-id="e40a6-103">Specifies what filter level of safe search is required.</span></span>
## <a name="members"></a><span data-ttu-id="e40a6-104">Membros</span><span class="sxs-lookup"><span data-stu-id="e40a6-104">Members</span></span>
|<span data-ttu-id="e40a6-105">Membro</span><span class="sxs-lookup"><span data-stu-id="e40a6-105">Member</span></span>|<span data-ttu-id="e40a6-106">Valor</span><span class="sxs-lookup"><span data-stu-id="e40a6-106">Value</span></span>|<span data-ttu-id="e40a6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e40a6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e40a6-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="e40a6-108">User-defined</span></span>|<span data-ttu-id="e40a6-109">0</span><span class="sxs-lookup"><span data-stu-id="e40a6-109">0%</span></span>|<span data-ttu-id="e40a6-110">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="e40a6-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e40a6-111">strict</span><span class="sxs-lookup"><span data-stu-id="e40a6-111">Strict</span></span>|<span data-ttu-id="e40a6-112">1</span><span class="sxs-lookup"><span data-stu-id="e40a6-112">-1</span></span>|<span data-ttu-id="e40a6-113">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="e40a6-113">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="e40a6-114">moderate</span><span class="sxs-lookup"><span data-stu-id="e40a6-114">Moderate:</span></span>|<span data-ttu-id="e40a6-115">2</span><span class="sxs-lookup"><span data-stu-id="e40a6-115">-2</span></span>|<span data-ttu-id="e40a6-116">Moderar filtragem em relação a conteúdo para adultos (resultados de pesquisa válidos não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="e40a6-116">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|








