-- Munch Solen — Hyprland theme surface.
--
-- Visual values only. Layout, binds, and input stay upstream.
-- Active windows wear the rays (cadmium → yellow → straw). Inactive
-- windows fall into the rock. A slow borderangle loop turns the gradient
-- like the disk; disable that leaf on battery if the redraw shows up.

local cadmium = "c44838"
local yellow = "c8b040"
local straw = "efe2bf"
local rock = "2b2e4a"
local cleft = "0e101c"

local active_border_color = {
	colors = {
		"rgba(" .. cadmium .. "ee)",
		"rgba(" .. yellow .. "ee)",
		"rgba(" .. straw .. "dd)",
	},
	angle = 90,
}
local inactive_border_color = "rgba(" .. rock .. "aa)"

hl.config({
	general = {
		col = {
			active_border = active_border_color,
			inactive_border = inactive_border_color,
		},
	},

	group = {
		col = {
			border_active = active_border_color,
			border_inactive = inactive_border_color,
		},
	},

	decoration = {
		shadow = {
			enabled = true,
			range = 16,
			render_power = 3,
			offset = "0 4",
			color = "rgba(" .. cleft .. "cc)",
			color_inactive = "rgba(" .. cleft .. "88)",
		},
	},
})

-- One full rotation of the ray gradient; speed 100 is Hyprland's slowest loop.
hl.animation({ leaf = "borderangle", enabled = true, speed = 100, bezier = "linear", style = "loop" })
