# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="d64c0-101">tipo enumerado automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d64c0-101">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="d64c0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d64c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d64c0-103">Valores possíveis para o modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="d64c0-103">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="d64c0-104">Membros</span><span class="sxs-lookup"><span data-stu-id="d64c0-104">Members</span></span>
|<span data-ttu-id="d64c0-105">Membro</span><span class="sxs-lookup"><span data-stu-id="d64c0-105">Member</span></span>|<span data-ttu-id="d64c0-106">Valor</span><span class="sxs-lookup"><span data-stu-id="d64c0-106">Value</span></span>|<span data-ttu-id="d64c0-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d64c0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d64c0-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="d64c0-108">User-defined</span></span>|<span data-ttu-id="d64c0-109">0</span><span class="sxs-lookup"><span data-stu-id="d64c0-109">0%</span></span>|<span data-ttu-id="d64c0-110">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="d64c0-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d64c0-111">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="d64c0-111">notifyDownload</span></span>|<span data-ttu-id="d64c0-112">1</span><span class="sxs-lookup"><span data-stu-id="d64c0-112">-1</span></span>|<span data-ttu-id="d64c0-113">Notificar ao baixar.</span><span class="sxs-lookup"><span data-stu-id="d64c0-113">Notify on download.</span></span>|
|<span data-ttu-id="d64c0-114">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d64c0-114">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="d64c0-115">2</span><span class="sxs-lookup"><span data-stu-id="d64c0-115">-2</span></span>|<span data-ttu-id="d64c0-116">Instalar automaticamente no período de manutenção.</span><span class="sxs-lookup"><span data-stu-id="d64c0-116">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="d64c0-117">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d64c0-117">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="d64c0-118">3</span><span class="sxs-lookup"><span data-stu-id="d64c0-118">-3</span></span>|<span data-ttu-id="d64c0-119">Instalar automaticamente e reinicializar no período de manutenção.</span><span class="sxs-lookup"><span data-stu-id="d64c0-119">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="d64c0-120">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="d64c0-120">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="d64c0-121">4</span><span class="sxs-lookup"><span data-stu-id="d64c0-121">-4</span></span>|<span data-ttu-id="d64c0-122">Instalar automaticamente e reinicializar no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="d64c0-122">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="d64c0-123">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="d64c0-123">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="d64c0-124">5</span><span class="sxs-lookup"><span data-stu-id="d64c0-124">$-5</span></span>|<span data-ttu-id="d64c0-125">Instalar automaticamente e reiniciar sem controle de usuário final</span><span class="sxs-lookup"><span data-stu-id="d64c0-125">Auto-install and restart without end-user control</span></span>|








